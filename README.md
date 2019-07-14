buttonlar = container.findViewById(R.id.buttonlar);
        text = container.findViewById(R.id.text);

        View view = inflater.inflate(R.layout.fragment_first, container, false);
        buttonlar = view.findViewById(R.id.buttonlar);
        buttonlar.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                text.setText("test");

            }
        });
        return view;
        
        
        Logcat
        
        2019-07-14 22:35:34.476 15349-15349/com.medicalsix.doctorsix E/chromium: [ERROR:gl_surface_egl.cc(342)] eglChooseConfig failed with error EGL_SUCCESS
    2019-07-14 22:35:38.959 15349-15349/com.medicalsix.doctorsix E/AndroidRuntime: FATAL EXCEPTION: main
    Process: com.medicalsix.doctorsix, PID: 15349
    java.lang.NullPointerException: Attempt to invoke virtual method 'void android.widget.TextView.setText(java.lang.CharSequence)' on a null object reference
        at com.medicalsix.doctorsix.First$1.onClick(First.java:48)
        at android.view.View.performClick(View.java:7251)
        at android.view.View.performClickInternal(View.java:7228)
        at android.view.View.access$3500(View.java:802)
        at android.view.View$PerformClick.run(View.java:27843)
        at android.os.Handler.handleCallback(Handler.java:883)
        at android.os.Handler.dispatchMessage(Handler.java:100)
        at android.os.Looper.loop(Looper.java:214)
        at android.app.ActivityThread.main(ActivityThread.java:7116)
        at java.lang.reflect.Method.invoke(Native Method)
        at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:492)
        at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:925)
