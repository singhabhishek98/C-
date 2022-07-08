/*
    Time Complexity : O(N!)
    Space Complexity : O(N^2)
    
    Where N is the number of queens.
*/

bool isSafe(vector < vector < int >> & board, int row, int col, int n) {
    
    int i;
    int j;

    // Check this row on left side.
    for (i = 0; i < col; i++) {
        if (board[row][i]) {
            return false;
        }
    }

    // Check upper diagonal on left side.
    for (i = row, j = col; i >= 0 && j >= 0; i--, j--) {
        if (board[i][j]) {
            return false;
        }
    }

    // Check lower diagonal on left side.
    for (i = row, j = col; j >= 0 && i < n; i++, j--) {
        if (board[i][j]) {
            return false;
        }
    }

    return true;
}

// Function to add valid configuration.
void addSolution(vector < vector < int >> & board, int n, vector < vector < int >> & ans) {
    vector < int > currentAnswer;
    for (auto x: board) {
        for (auto y: x) {
            currentAnswer.push_back(y);
        }
    }
    ans.push_back(currentAnswer);
}

void solve(vector < vector < int >> & board, int col, int n, vector < vector < int >> & ans) {
    // All queens placed.
    if (col >= n) {
        addSolution(board, n, ans);
        return;
    }

    for (int i = 0; i < n; i++) {
        if (isSafe(board, i, col, n)) {
            board[i][col] = 1;
            solve(board, col + 1, n, ans);
            board[i][col] = 0;
        }
    }

    return;
}

vector < vector < int >> solveNQueens(int n) {
    vector < vector < int >> board(n, vector < int > (n, 0));
    vector < vector < int >> ans;
    solve(board, 0, n, ans);
    return ans;
}
