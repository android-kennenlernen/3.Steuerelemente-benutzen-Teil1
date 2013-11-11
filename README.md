# 3. Steuerelemente einbringen

[In Aufbau]

Hier erfolgen nun die Hinweise zur Erstellung einer Nutzer-Oberfläche.

----

__Hilfestellung__

Zunächst ist ein neues Android-Projekt erstellen.

Dann wird im Projekt-Verzeichnis zu  
**res/layout/activity_main.xml**
gewechselt.

Wenn Ihr auf diesen Dateinamen klickt, öffnet sich das 'Graphical Layout'.  

Nun werden mittels dieses Oberflächen-Designer

- 1 EditText
- 1 TextView
- 1 Schalter namens 'btnDrueckDochMal'
- 1 Schalter namens 'btnRaeumeAuf'
in die Oberfläche der Activity eingebracht.

Nach dem Einbringen der Steuerelemente sollte die **activity_main.xml** nun so aussehen:

```xml
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:paddingBottom="@dimen/activity_vertical_margin"
    android:paddingLeft="@dimen/activity_horizontal_margin"
    android:paddingRight="@dimen/activity_horizontal_margin"
    android:paddingTop="@dimen/activity_vertical_margin"
    tools:context=".MainActivity" >

    <EditText
        android:id="@+id/editText1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentLeft="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentTop="true"
        android:layout_marginTop="30dp"
        android:ems="10" />

    <TextView
        android:id="@+id/textView1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignLeft="@+id/editText1"
        android:layout_alignParentRight="true"
        android:layout_below="@+id/editText1"
        android:layout_marginTop="31dp"
        android:text="TextView" />

    <Button
        android:id="@+id/btnDrueckDochMal"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignLeft="@+id/textView1"
        android:layout_below="@+id/textView1"
        android:layout_marginTop="30dp"
        android:text="Drück doch mal" />

    <Button
        android:id="@+id/btnRaeumeAuf"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignBaseline="@+id/btnDrueckDochMal"
        android:layout_alignBottom="@+id/btnDrueckDochMal"
        android:layout_marginLeft="14dp"
        android:layout_toRightOf="@+id/btnDrueckDochMal"
        android:text="Räume auf" />

</RelativeLayout>
```

Was sollten wir nun beherrschen?

- Einbringen von Steuerelementen
- Vergabe von selbstgewählten Bezeichnern für dieselben