#include <bits/stdc++.h>
using namespace std;

typedef long long LL;
typedef pair<int, int> II;

int main() {
    #ifdef LOCAL
        freopen("Data.inp", "r", stdin);
        freopen("Data.out", "w", stdout);
    #endif

    int n, a[100];
    cin >> n;
    for (int i = 1; i <= n; ++i) cin >> a[i];

    for (int i = 1; i <= n; ++i) {
        for (int j = 1; j <= n; ++j) if (a[a[j]] == i) {
            cout << j << endl;
            break;
        }
    }

    return 0;
}
