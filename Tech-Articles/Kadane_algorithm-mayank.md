
=======================================================

Article Title: <Kadane's Algorithm>
Author Name: <Mayank Johari>
Author Profile: https://github.com/mayankmj
Date: 20/Oct/2021

=======================================================

Kadane’s Algorithm:
Time complexity O(n)
Explanation: 
            Kadane’s algorithm look for all positive continuous segments of the one dimensional array and keep the sum stored in an variable (let say "current") . in each 
            iteration if we get positive sum , compare and put it to variable (let say "maximum") , if current gets negative assign current to zero.. after 'n' iterations we 
            get the maximum continuous subarray sum in "maximum" variable
Sample CPP Code 


#include <bits/stdc++.h>
using namespace std;
#define int long long
#define pi (3.141592653589)
#define mod 1000000007
#define int long long
#define float double
#define pb push_back
#define mp make_pair
#define ff first
#define ss second
#define all(c) c.begin(), c.end()
#define min3(a, b, c) min(c, min(a, b))
#define min4(a, b, c, d) min(d, min(c, min(a, b)))
#define rrep(i, n) for(int i=n-1;i>=0;i--)
#define rep(i,n) for(int i=0;i<n;i++)
#define array_input(n,arr) for(int i=0;i<n;i++) cin>>arr[i] 
#define array_output(n,arr) for(int i=0;i<n;i++) cout<<arr[i]
#define debug1(x) cout<<x<<endl 
#define debug2(x,y) cout<<x<<y<<endl  
#define debug3(x,y,z) cout<<x<<y<<z<<endl 
#define fast ios_base::sync_with_stdio(false), cin.tie(nullptr), cout.tie(nullptr);
int32_t main(){
fast
//TAKING NUMBER OF TEST CASES
int t=1;
cin>>t;
while(t--){
    int n;
    //SIZE OF ARRAY
    cin>>n;
    int arr[n];
    //INPUT ARRAY
    array_input(n,arr);
    int maximum=0,current=0;
    for(int i=0;i<n;i++)
    {
        current=current+arr[i];
        if(current>maximum)
        maximum=current;
        if(current<0)
        current=0;
    }
    //SUM OF MAXIMUM CONTINUOUS SUBARRAY
    cout<<maximum<<endl;
}
return 0;
}


