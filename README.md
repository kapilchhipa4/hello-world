# hello-world
it will show how to print hello world in python.
now i am making some changes.



1.  create a repositery in which u want to upload your project.
2. type in gitbash 'git init' ( inside your project folder which u want to upload)
3. then type 'git remote add origin https://github.com/kapilchhipa4/game-in-javascript.git' (it is the link of your repositery)
4.  git remote -v  ( check origin)
5. git add . ( it will add all the files of your folder)
6. git commit -m "some message"  ( commit the changes)
7. git  push -f origin master   ( now u can push on origin )
8 done;




make new branch and upload updated project------------

1.  type in gitbash 'git init' ( inside your project folder which u want to upload)
2. then type 'git remote add origin https://github.com/kapilchhipa4/game-in-javascript.git' (it is the link of your repositery)
3. git remote -v  ( check origin)
4. git checkout -b new-branch-name
5. git add . ( it will add all the files of your folder)
6. git commit -m "some message"  ( commit the changes)
7. git  push -f origin 'your branch name'   ( now u can push on origin )



E: Could not get lock /var/lib/dpkg/lock - open (11: Resource temporarily unavailable)
E: Unable to lock the administration directory (/var/lib/dpkg/), is another process using it?

fix that error

1. ps aux | grep -i apt
2. kill process with 'kill process_id' command 
 2.1 sudo kill -9 <process_id>  ( to kill forcefully)
 2.2 sudo killall apt apt-get ( to kill all process)
























#include<bits/stdc++.h>
typedef long long ll;
typedef double ld;
#define vll vector<ll>
#define vvll vector< vll >
#define vld vector< ld >
#define vvld vector< vld >
#define pll pair<ll ,ll >
#define vllp vector< pll >
#define mp make_pair
#define pb push_back
#define MOD 1000000007
#define endl "\n"
#define test ll t;cin>>t;while(t--)
#define all(v) v.begin(),v.end()
#define rall(v) v.rbegin(),v.rend()
#define F first
#define S second

#define forn(i,n) for(ll (i) = 0 ; (i) < (n) ; ++(i))
#define for1(i,n) for(ll (i) = 1 ; (i) <= (n) ; ++(i))
#define forr(i,n) for(ll (i) = (n)-1 ; (i)>=0 ; --(i))
#define forab(i,a,b,c) for(ll (i) = a ; (i) <= (b) ; (i)+=(c))
#define MAX 1000000007
using namespace std;

vll sieve;
void Sieve(int N){
 const ll maxn = N;
 sieve.resize(maxn);
 forn(i,maxn) sieve[i] = i;
 sieve[1] = -1;
 sieve[0] = -1;
 forab(i,2,maxn,1) if(i == sieve[i]) for(ll j = 2*i ; j < maxn ; j+=i) if(sieve[j] == j) sieve[j] = i;
}
ll extended_GCD(ll a , ll b , ll &x , ll &y){
 if(a == 0){
     x = 0;
     y = 1;
     return b;
 }
 ll x1 , y1;
 ll gcd = extended_GCD(b%a , a , x1 , y1);
 x = y1 - (b/a)*x1; 
 y = x1;
 return gcd;
}
ll power(ll a, ll b, ll m = MOD) {
    a %= m;
    ll res = 1;
    while (b > 0) {
        if (b & 1)
            res = res * a % m;
        a = a * a % m;
        b >>= 1;
    }
    return res;
}
ll modinv(ll a , ll mod = MOD){
 ll x , y;
 extended_GCD(a , mod , x , y);
 if(x < 0) x += mod;
 return x;
}
