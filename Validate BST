# Soltion of
- Validate BST
- `https://leetcode.com/problems/validate-binary-search-tree/description/`


class Solution(object):
    def isValidBST(self, root):
        """
        :type root: TreeNode
        :rtype: bool
        """
        def isBSTUtil(node, min_val, max_val):
            if node is None:
                return True
            
            if min_val is not None and node.val <= min_val:
                return False
            
            if max_val is not None and node.val >= max_val:
                return False
            
            return (
                isBSTUtil(node.left, min_val, node.val) and
                isBSTUtil(node.right, node.val, max_val)
            )
        
        return isBSTUtil(root, None, None)
        
        
- Leetcode: `https://leetcode.com/problems/validate-binary-search-tree/submissions/950242613/`
