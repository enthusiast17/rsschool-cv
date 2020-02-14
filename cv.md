# CV

Ulan Nurym
---
### Contact Info
Email: ulan17nurym@gmail.com

---
### Summary
I am an enthusiastic and curious person. I've never explore frontend development. So the `RS School` is really good start for me. Also, I am interested in dev tools. I think, javascript language will help me to create some tools and scripts. I hope I will get good experience. Good luck to me.

---
### Skills
- Go
- Java (Android)
- Basic HTML and CSS
- Bash

---
### Code example
```Go
    package student

    func Min(root *TreeNode) *TreeNode {
    	if root == nil {
    		return root
    	}
    	it := root
    	for it.Left != nil {
    		it = it.Left
    	}
    	root = it
    	return root
    }

    func BTreeDeleteNode(root, node *TreeNode) *TreeNode {
    	if root == nil || node == nil {
    		return root
    	}

    	if node.Left == nil {
    		root = BTreeTransplant(root, node, node.Right)
    	} else if node.Right == nil {
    		root = BTreeTransplant(root, node, node.Left)
    	} else {
    		minBTree := Min(node.Right)
    		if minBTree.Parent != node {
    			root = BTreeTransplant(root, minBTree, minBTree.Right)
    			minBTree.Right = node.Right
    			minBTree.Right.Parent = minBTree
    		}
    		root = BTreeTransplant(root, node, minBTree)
    		minBTree.Left = node.Left
    		minBTree.Left.Parent = node
    	}

    	return root
    }
```
---
### Exprience
- f3s - parse flags from args, [Git](https://github.com/enthusiast17/f3s)
- TimeTable - an android app for students, [Git](https://github.com/ulan17/timetable)

---
### Education
- Alem school, 2019-current
- HTMLAcademy, 2020, HTML&CSS

---
### English
Pre-intermediate (А2)
