#include <map>
#include <set>
#include <list>
#include <cmath>
#include <ctime>
#include <deque>
#include <queue>
#include <stack>
#include <string>
#include <bitset>
#include <cstdio>
#include <limits>
#include <vector>
#include <climits>
#include <cstring>
#include <cstdlib>
#include <fstream>
#include <numeric>
#include <sstream>
#include <iostream>
#include <algorithm>
#include <unordered_map>

using namespace std;
void sum(int arr[],int n)
{
    int i,s=0,max=0;
    for(i=0;i<n;i++)
    {
        s=s+arr[i];
        if(s>max)
        {
            max=s;
        }
        if(s<0)
        {
            s=0;
        }
    }
    cout<<max;
}
int main() {
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */
    int n,i;
    cin>>n;
    int arr[n];
    for(i=0;i<n;i++)
    {
        cin>>arr[i];
    }
    sum(arr,n);
    return 0;
}
