# Result
For $i = 1 To 5     $s &amp;= Random(100, 1000, 1)     $s &amp;= @LF &amp; Random(100, 1000, 1)     For $j = 1 To 10         $s &amp;= @CRLF     Next Next  MsgBox(0, "Original", $s) MsgBox(0, "Result", StringRegExpReplace($s, '(\n[^\n]+)(?=\n)(?=.*?\1)', ""))
