# Func-_ErrADODB-Msgbox-0-ADODB-COM-Error-We-intercepted-a-COM-Error-CRLF-CRLF
EndFunc  Func _ErrADODB()     Msgbox(0,"ADODB COM Error","We intercepted a COM Error !"      &amp; @CRLF  &amp; @CRLF &amp; _              "err.description is: "    &amp; @TAB &amp; $errADODB.description    &amp; @CRLF &amp; _              "err.windescription:"     &amp; @TAB &amp; $errADODB.windescription &amp; @CRLF &amp; _              "err.number is: "         &amp; @TAB &amp; hex($errADODB.number,8)  &amp; @CRLF &amp; _              "err.lastdllerror is: "   &amp; @TAB &amp; $errADODB.lastdllerror   &amp; @CRLF &amp; _              "err.scriptline is: "     &amp; @TAB &amp; $errADODB.scriptline     &amp; @CRLF &amp; _              "err.source is: "         &amp; @TAB &amp; $errADODB.source         &amp; @CRLF &amp; _              "err.helpfile is: "       &amp; @TAB &amp; $errADODB.helpfile       &amp; @CRLF &amp; _              "err.helpcontext is: "    &amp; @TAB &amp; $errADODB.helpcontext _             )     Local $err = $errADODB.number     If $err = 0 Then $err = -1 EndFunc    #include &lt;Array.au3>   ;Only needed for This Demo Script  $adCurrentProvider = $adProviderMSJET4   ;Microsoft.Jet.OLEDB.4.0 $adCurrentDataSource = @ScriptDir &amp; "\TEMPDB.MDB"
