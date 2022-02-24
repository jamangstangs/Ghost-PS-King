## 1330

```c++
#include<iostream>
using namespace std;

int main(){
	int a,b;
  cin >> a >> b;
  
  if(a>b) cout << ">";
  else if(a<b) cout << "<";
  else cout << "==";
}

#include<iostream>
using namespace std;

int main(){
	int a,b;
  cin >> a >> b;
  
  a>b?cout<<">":(a<b?cout<<"<":cout<<"==");
}
```

- 3항 연산자의 활용

## 9498

````c++
#include<iostream>
using namespace std;
int main(){int a; cin >> a; (100>=a&&a>=90)?cout<<"A":(89>=a&&a>=80)?cout<<"B":(79>=a&&a>=70)?cout<<"C":(69>=a&&a>=60)?cout<<"D":cout<<"F";}
````

## 2753

```c++
#include<iostream>
using namespace std;

int main(){
  int a;
	cin>>a;
  ((a%4==0)&&(a%100!=0))||(a%400==0)?cout<<1:cout<<0;
}
```

## 14681

```c++
#include<iostream>
using namespace std;int main(){int x,y;cin>>x>>y;(x*y>0)?((x>0)?cout<<1:cout<<3):((x>0)?cout<<4:cout<<2);}
```

## 2884

```c++
#include<iostream>
using namespace std;int main(){int a,b;cin >>a>>b;a*=60;a+=b;a-=45;if(a<0) a+=1440;b=a%60;a/=60;cout<<a<<" "<<b;}

```

## 2525

```c++
  #include<iostream>
  using namespace std;

  int main(){
    int a,b,c,t;
    cin>>a>>b>>c;
    t = ((a*60+b)+c)%1440;
    a = t/60;
    b = t%60;
    cout<<a<<" "<<b;
  }
```

## 2480

```c++
#include<iostream>
using namespace std;
int main(){
    int a,b,c;
    cin >> a >> b >> c;
    if(a==b && b==c) cout << a*1000+10000;
    else if (a==b) cout << a*100+1000;
    else if (c==b) cout << c*100+1000;
    else if (a==c) cout << c*100+1000;
    else (a>b)?((a>c)?cout<<a*100:cout<<c*100):((b>c)?cout<<b*100:cout<<c*100);
}
```

- 삼항 연산자를
- cout<<(a>b)?((a>c)?cout<<a*100:cout<<c*100):((b>c)?cout<<b*100:cout<<c*100); 이렇게 쓰니까 틀리지..