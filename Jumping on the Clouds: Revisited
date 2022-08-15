#include <bits/stdc++.h>

#define FO(i,a,b) for (int i = (a); i < (b); i++)
#define sz(v) int(v.size())

using namespace std;

int n, k, e;
int t[105];

int main() {
    scanf("%d %d", &n, &k); e = 100;
    FO(i,0,n) scanf("%d", t+i);
    int i = 0;
    while (1) {
        e -= 2*t[i]+1;
        i = (i+k)%n;
        if (i == 0) break;
    }
    printf("%d\n", e);
}
