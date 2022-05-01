# don-t-touch-my-code
 Warum sie überhaupt gebraucht wird, denke ich, 

 Sie wissen es selbst, wenn Sie auf diesen Artikel stoßen. Sie wollen nicht, dass Ihr Code von irgendjemandem eingesehen werden kann! Zu diesem Zweck müssen Sie bestimmte Aktionen auf der Website verbieten:

 1. den Besuchern verbieten, die rechte Taste zu benutzen - sie deaktivieren.
 2. Verhindern Sie, dass ein Besucher den Seitencode sehen kann.
 3. Verbot von Code-Reviews oder anderen Untersuchungen eines Elements.

 Alle drei Aktionen müssen zusammen deaktiviert werden. Der obige Skriptcode erledigt das alles!
        document.oncontextmenu - deaktiviert die rechte Maustaste. 

 Aber das reicht nicht aus, denn es ist möglich, ein Element zu erkunden und den Seitencode mit einem Tastaturkürzel anzuzeigen. Daher müssen wir auch diese Funktion deaktivieren.

 event.keyCode == 85 - deaktiviert die Tastenkombination ctrl+U
 event.keyCode == 73 - deaktiviert die Tastenkombination ctrl+shift+i
 event.keyCode == 73 - deaktiviert die Tastenkombination F12

 JavaScript kann verwendet werden, um eine beliebige Taste oder Tastenkombination auf der Website zu deaktivieren, z. B. ctrl+C - event.keyCode == 67
