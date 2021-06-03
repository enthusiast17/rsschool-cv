# CV

Ulan Nurym
---
### Contact Info
Email: ulan17nurym@gmail.com

---
### Summary
I am an enthusiastic and curious person. I've never explored frontend development. So the `RS School` is really good start for me. Also, I am interested in dev tools. I think, JavaScript language will help me to create some dev tools and scripts. I hope I will get a good experience. Good luck to me.

---
### Skills
- Go
- Java (Android)
- Basic HTML and CSS
- Bash
- Git, Github

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
- TimeTable - an android application for students, [Git](https://github.com/ulan17/timetable)

---
### Education
- alem school, 2019 - current
- HTML Academy, 2020

---
### Languages
- Kazakh - Native
- Russian - Fluent
- English - Pre-intermediate (А2)
