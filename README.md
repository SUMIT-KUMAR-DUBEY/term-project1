#include <iostream>
#include<condition_variable>
using namespace std;

class cal
{
  private:
  int num,i,j,beta,alpha,sum,n;
  public:
  cal()
  { sum=0;
     i=0;
    j=0;
  }
  ~cal()
  {
    cout<<endl;
    cout<<"Thankyou";

  }

  void input()
  {  cout<<"Enter your number (input) =";
     cin>>num;

  }
  void calculate()
  { alpha = num;
    while(alpha!=0)
   { 
     alpha = alpha/2;
     i++;
    }
  
   int binary[i];
   beta=num;

   while(beta!=0)
     {
       binary[j]=beta%2;
       
       beta=beta/2;
       
      
       if(binary[j]==1)
       sum++;
       j++;
     } 
    
  }

   void output()
      {  
        cout<<endl<<"Output="<<sum;
        
      }
};
int main()
{
  cal value;
  value.input();
  value.calculate();
  value.output();

  return 0;

}      



  




  // int num,i,j,beta,alpha,sum;
  // cout<<"Enter your number";
  // cin>>num;
  // sum=0;
  // i=0;
  // j=0;
  
  // alpha = num;
  // while(alpha!=0)
  // { 
  //    alpha = alpha/2;
  //    i++;

  // }
  
  //  int binary[i];
  //  beta=num;

  // while(beta!=0)
  // {
  //      binary[j]=beta%2;
  //      beta=beta/2;
  //      if(binary[j]==1)
  //      sum++;
  //      j++;
       
  // }



 // cout<<"Total 1 in binar  representation"<<sum;
 // return 0;


