#include <bits/stdc++.h>

using namespace std;

int a[42];
char s[1231212];

int main() {
  for (int i = 0; i < 26; i++) {
    scanf("%d", a + i);
  }
  scanf("%s", s);
  int h = 0;
  int w = 0;
  for (int i = 0; s[i]; i++) {
    w++;
    h = max(h, a[s[i] - 'a']);
  }
  printf("%d\n", h * w);
  return 0;
}
