# Login

LogIn-en-Android-Studio-con-SQLite

Hola Skriom, desearia saber si puedes ayudarme a solucionar el error que en general presentan todos los usuario de tu canal, Leonor Romero en tu ultimo video indica lo relacionado a los metodos llamados getUsuario() y setUsuario(), el cual considero que puede ser el problema pero no he logrado solucionarlo. Gracias¡¡

---------- El primer error corresponde a la siguiente linea de Inicio.java: 
nombre.setText(u.getNombre()+""+u.getApellidos());

02-07 10:51:03.412 16723-16723/com.example.login E/AndroidRuntime: FATAL EXCEPTION: main Process: com.example.login, PID: 16723 java.lang.RuntimeException: Unable to start activity ComponentInfo{com.example.login/com.example.login.Inicio}: java.lang.NullPointerException: Attempt to invoke virtual method 'java.lang.String com.example.login.Usuario.getNombre()' on a null object reference at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:2416) at android.app.ActivityThread.handleLaunchActivity(ActivityThread.java:2476) at android.app.ActivityThread.-wrap11(ActivityThread.java) at android.app.ActivityThread$H.handleMessage(ActivityThread.java:1344) at android.os.Handler.dispatchMessage(Handler.java:102) at android.os.Looper.loop(Looper.java:148) at android.app.ActivityThread.main(ActivityThread.java:5417) at java.lang.reflect.Method.invoke(Native Method) at com.android.internal.os.ZygoteInit$MethodAndArgsCaller.run(ZygoteInit.java:726) at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:616) Caused by: java.lang.NullPointerException: Attempt to invoke virtual method 'java.lang.String com.example.login.Usuario.getNombre()' on a null object reference at com.example.login.Inicio.onCreate(Inicio.java:39) at android.app.Activity.performCreate(Activity.java:6237) at android.app.Instrumentation.callActivityOnCreate(Instrumentation.java:1107) at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:2369)

-------- El segundo error considero que es consecuencia del primero y es en la siguinetes lineas de Editar.java:

ediUser.setText(u.getUsuario());
ediPass.setText(u.getPassword()); 
ediNombre.setText(u.getNombre()); 
ediApellido.setText(u.getApellidos());

02-07 11:03:53.205 16854-16854/com.example.login E/AndroidRuntime: FATAL EXCEPTION: main Process: com.example.login, PID: 16854 java.lang.RuntimeException: Unable to start activity ComponentInfo{com.example.login/com.example.login.Editar}: java.lang.NullPointerException: Attempt to invoke virtual method 'java.lang.String com.example.login.Usuario.getUsuario()' on a null object reference at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:2416) at android.app.ActivityThread.handleLaunchActivity(ActivityThread.java:2476) at android.app.ActivityThread.-wrap11(ActivityThread.java) at android.app.ActivityThread$H.handleMessage(ActivityThread.java:1344) at android.os.Handler.dispatchMessage(Handler.java:102) at android.os.Looper.loop(Looper.java:148) at android.app.ActivityThread.main(ActivityThread.java:5417) at java.lang.reflect.Method.invoke(Native Method) at com.android.internal.os.ZygoteInit$MethodAndArgsCaller.run(ZygoteInit.java:726) at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:616) Caused by: java.lang.NullPointerException: Attempt to invoke virtual method 'java.lang.String com.example.login.Usuario.getUsuario()' on a null object reference at com.example.login.Editar.onCreate(Editar.java:40) at android.app.Activity.performCreate(Activity.java:6237) at android.app.Instrumentation.callActivityOnCreate(Instrumentation.java:1107) at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:2369)

    https://www.youtube.com/watch?v=JrjnflOy2tY&t=9s
    https://www.youtube.com/watch?v=cGmZ1wwOyZQ&t=181s
    https://www.youtube.com/watch?v=r2hs9OuWZOs
    https://www.youtube.com/watch?v=n10SRistBVg&t=1276s
