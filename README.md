小组成员：王家鹏

账户名称：123rtkgrtj

项目简介：实现merkle树

项目名称：merkle-tree

完成人：王家鹏

代码说明：

    merkle树是一种用于加密和哈希的二叉树，其中叶节点为要压缩的消息。
    
    实现时首先要将消息进行划分为n组。
    
    对于每一组消息m’，计算它的哈希值，然后每两个哈希值组成一组级联起来，再次进行哈希。
    
    以此类推，直到最后生成最终的一个哈希值，即为整个消息的压缩结果。
    
    若消息不能两两划分完，则将最后一个消息的节点记录下来，并以它为头节点对应的树上的所有节点高度均加一作为下一层节点进行。
    
    相关函数说明：
    
    print_tree():用于打印出整个merkle树
    
    hash()：计算单个消息的哈希值
    
    hash_nodes():计算两个消息级联后的哈希值
    
    last_node():找出markle树中的最后一个节点
    
    find_new_node():找出可插入的节点
    
    initial():生成merkle树
    
    delete_tree():删除merkle_tree
    
    devide_string():划分消息
    
    delete_string():删除消息
    
运行结果：

    ![image](https://user-images.githubusercontent.com/110152761/182010944-ac4f2ce7-5949-4043-ba36-61b40d335eea.png)

    
    
