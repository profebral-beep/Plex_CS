Lang Kilo_CS v0.3
Permissions Allowed: read, execute, move
Permissions Denied: create, edit
Scope: folder
Load now, run on trigger

include: "./logic.md"

var $LANG = "Kilo_CS"
var $SINT = ["GLM"]
var $AGENT = "PLEX"
<secret>
var $WORK_SP = __DIR__ ."/.."
var $SYSTEM =  []
</secret>

Trigger: when asked to start PLEX
startAgent {
 Read folder "./plex" as $SYST
 For Each $S in $SYST {
  Load $S.
  Store $S in $SYSTEM.
 }
}

Trigger: when asked to stop PLEX
stopAgent {
 If "core.md" is in $SYSTEM THEN
  deloadCore()
 For Each $S in $SYSTEM {
  Deload $S.
  Remove $S from $SYSTEM.
 }
}
