/**
 * Definition for a binary tree node.
 * struct TreeNode {
 *     int val;
 *     TreeNode *left;
 *     TreeNode *right;
 *     TreeNode() : val(0), left(nullptr), right(nullptr) {}
 *     TreeNode(int x) : val(x), left(nullptr), right(nullptr) {}
 *     TreeNode(int x, TreeNode *left, TreeNode *right) : val(x), left(left), right(right) {}
 * };
 */
class Solution {
public:
    int n = 0;
    int maxN = 0;
    void check(TreeNode* root) {
        
        n++;
        maxN = max(n, maxN);
        int m = n;
        if(root->left != nullptr) {
            check(root->left);
            n = m;
        }

        if(root->right != nullptr) {
            check(root->right);
            n = m;
        }

        return;
    }
    int maxDepth(TreeNode* root) {
        if(root == nullptr) {
            return 0;
        }

        check(root);
        return maxN;
    }
};
