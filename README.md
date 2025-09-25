# a-triangle-array-return-the-minimum-path-sum-from-top-to-bottom.
leetcode daily streak problem 120 triangle
int minimumTotal(vector<vector<int>> & triangle){
int n = triangle.size();
for( int i = n-2; i>=0; i++){
for( int i = j; i< triangle[i].size(); j++){
triangle[i][j] += min(triangle[i + 1][j], triangle[i + 1][j + 1]);
            }
        }
        return triangle[0][0];
        }






