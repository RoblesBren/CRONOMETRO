# CRONOMETRO

#include <string>
#include <ctime>
#include <cstdlib>
#include <iostream>

using namespace std;

int main()


{

    int hr;
    int minu;
    int seg;
    int tim;
    int c;
    int ms;
    int x;
    string tiempo;
    cout<<"introduce el tiempo con el formato HH:MM:SS";
    cin>>tiempo;
    string hora = tiempo.substr (0,2);
    string minuto = tiempo.substr (3,2);
    string segundo = tiempo.substr (6,2);

    hr = atoi (hora.c_str());
    minu = atoi (minuto.c_str());
    seg = atoi (segundo.c_str());
    tim = atoi (tiempo.c_str());

x==1;
    while(x==1);
    {


        for(ms=0;ms<1000;ms++)
        {
            if(ms==1000){ms=0,seg--;}
            if(seg==0){seg=60,minu--;}
            if(minu==0){minu=60,hr--;}
            cout<<hr<<":"<<minu<<":"<<seg<<endl;

        }

        for(seg=0;seg<60;seg++)
        {
            if(ms==0){ms=1000,seg--;}
            if(seg==60){seg=60,minu--;}
            if(minu==0){minu=60,hr--;}
            cout<<hr<<":"<<minu<<":"<<seg<<endl;

        }



        for(minu=0;minu<60;minu++)
        {
            if(ms==0){ms=1000,seg--;}
            if(seg==0){seg=60,minu--;}
            if(minu==60){minu=0,hr--;}
            cout<<hr<<":"<<minu<<":"<<seg<<endl;
        }

         for(hr=0;hr<24;hr++){
            if(ms==0){ms=1000,seg--;}
            if(seg==0){seg=60,minu--;}
            if(minu==0){minu=60,hr--;}
            if(minu==24){hr=0,hr--;}

            cout<<hr<<":"<<minu<<":"<<seg<<endl;

        }


    }

}



 for(seg=0;seg>0;seg++)
        {


            if(hr<10 && minu<10 && seg<10)
            {
                cout<<"0"<<hr<<":"<<"0"<<minu<<":"<<"0"<<seg<<endl;
            }
            else if(minu<10 && seg<10)
            {
                    cout<<hr<<":"<<"0"<<minu<<":"<<"0"<<seg<<endl;
            }
            else if(seg<10)
            {
                    cout<<hr<<":"<<minu<<":"<<"0"<<seg<<endl;
            }
            else if(hr<10 && seg<10)
            {
                    cout<<"0"<<hr<<":"<<minu<<":"<<"0"<<seg<<endl;
            }
            else if(hr<10 && minu<10 )
            {
                    cout<<"0"<<hr<<":"<<"0"<<minu<<":"<<seg<<endl;
            }
            else if(minu<10)
            {
                    cout<<hr<<":"<<"0"<<minu<<":"<<seg<<endl;
            }
            else if(hr<10)
            {
                    cout<<"0"<<hr<<":"<<minu<<":"<<seg<<endl;
            }
            else
            {
                    cout<<hr<<":"<<minu<<":"<<seg<<endl;
            }
        }
        if(minu==0)
        {
           if(hr==0)
           {
               x==0;
           }
