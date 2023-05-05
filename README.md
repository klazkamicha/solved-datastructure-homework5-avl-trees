Download Link: https://assignmentchef.com/product/solved-datastructure-homework5-avl-trees
<br>
You are required to implement an AVL tree. An AVL is a special type of binary search tree that follows all the same rules: each node has 0-2 children, all data in the left subtree is less than the node’s data, and all data in the right subtree is greater than the node’s data. The AVL differs from the BST with its own self-balancing rotations, which you must implement.

All methods in the AVL tree that are not O(1) <strong>must be implemented recursively</strong>. Good recursion with simple, focused states is strongly encouraged for this assignment in particular.

Your AVL tree will have two constructors: a no-argument constructor (which should initialize an empty tree), and a constructor that takes in data to be added to the tree, and initializes the tree with this data. <strong>Balancing</strong>

Each node has two additional instance variables, height and balanceFactor. The height variable should represent the height of the node (recall that a node’s height is max(child nodes’ heights)+1. The balance factor of a node should be equal to its left child’s height minus its right child’s height. The tree should rotate appropriately to make sure it’s always balanced. Keep in mind that you will have to update these instance variables; they are not updated automatically.

<h2>BST to AVL</h2>

You are encouraged to use your BST code as a base to get started on this homework. The main changes will occur in the add and remove methods since that’s where the structure of the tree can change. <strong>One notable change you should make besides the rotation logic is change the </strong>remove <strong>method to use the predecessor rather than the successor</strong>. This is not generally necessary in an AVL, but we thought it’d be good practice. Another method to make changes to is the height method since it’s no longer necessary to recalculate the height of the tree since it’s already been stored. We’ve also added a successor method that should get the successor of any data in the tree, not just in the two child case. This method is just for practice, and <strong>you should not be using it in any other methods</strong>.