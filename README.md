# Ud2_Ejemplo7
_Ejemplo 7 de la Unidad 2._ 

Vemos un ejemplo de cómo posicionar elementos relativos al padre en _RelativeLayout_ haciendo uso de los atributos _layout_alignParentRight_,
_layout_alignParentLeft_, _layout_alignParentRight_ y _layout_alignParentTop_. 


Sólo hemos de fijarnos en el fichero _activity_main.xml_:

```
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@android:color/darker_gray"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentRight="true"
        android:layout_alignParentTop="true"
        android:text="@string/uno"
        android:textColor="@android:color/white"
        android:textStyle="bold"/>

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentBottom="true"
        android:layout_alignParentRight="true"
        android:text="@string/dos"
        android:textColor="@android:color/white"
        android:textStyle="bold"/>

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentBottom="true"
        android:layout_alignParentLeft="true"
        android:text="@string/tres"
        android:textColor="@android:color/white"
        android:textStyle="bold"/>

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="@string/cuatro"
        android:textColor="@android:color/white"
        android:textStyle="bold"/>
</RelativeLayout>
```

Los textos de los _TextView_ se han insertado en el fichero _values/strings.xml_ y accedemos a ellos usando el símbolo @:

```
<resources>
    <string name="app_name">Ud2_Ejemplo7</string>
    <string name="uno">Uno</string>
    <string name="dos">Dos</string>
    <string name="tres">Tres</string>
    <string name="cuatro">Cuatro</string>
</resources>
```

Notad como en el _TextView_ con el texto _Cuatro_ no se ha usado ninguno de estos atributos y por defecto se ha posicionado en la
esquina superior izquierda.
