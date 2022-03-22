# Codeforcescpp-262A
#include <bits/stdc++.h>

using namespace std;

int main()
{
  int n,k,num,count(0);
  cin >> n >> k;
  for(int i=0;i<n;i++){
    cin >> num;
    int j = 1,tmp = 0;
    while((num/j)!=0){
      if(((num/j)%10)==4 || ((num/j)%10)==7){
        tmp++;
      }
      j*=10;
    }
    if(tmp<=k)
      count++;
  }
  cout << count;
  return 0;
}
