#include <bits/stdc++.h>
using namespace std;

int main() {
	int n, m;
	cin >> n >> m;
	vector<int> v;
	int ans = 0;
	for (int i = 0; i < n; i++) {
		int n = 0;
		for (int j = 0; j < m; j++){
			int t;
			cin >> t;
			n = max(n ,t);
		}
		v.push_back(n);
		ans += n;
	}
	cout << ans << '\n';
	int e = 0;
	vector<int> r;

	for (int i = 0; i < v.size(); i++) {
		if (ans % v[i] == 0) {
			r.push_back(v[i]);
		}
	}
	if (r.size() == 0) {
		cout << -1;
		return 0;
	}

	for (int i = 0; i < r.size() - 1; i++) {
		cout << r[i] << ' ';
	}
	cout << r[r.size() - 1];
}
