# GUIEdit
nclude &lt;IE.au3> #include &lt;GUIEdit.au3> #include &lt;Clipboard.au3> #include &lt;MsgBoxConstants.au3> #include &lt;GDIPlus.au3> #include &lt;Memory.au3> #include &lt;Misc.au3> #include &lt;DateTimeConstants.au3> #include &lt;File.au3> #include &lt;ColorConstants.au3>    ;~ **** Progress bar function goes here  Opt("TrayMenuMode", 3)  RAIS()  Func RAIS()     Local $iServices = TrayCreateMenu("Services")     Local $iLogin = TrayCreateItem("Login", $iServices)     Local $iDataEntry = TrayCreateItem("Data Entry", $iServices)      TrayCreateItem("")     Local $LSettings = TrayCreateItem("Login Settings")     Local $DSettings = TrayCreateItem("Default Settings")     Local $iAbout = TrayCreateItem("About")     TrayCreateItem("")     Local $iExit = TrayCreateItem("Exit")     TraySetIcon($icon)     TraySetState(1)
