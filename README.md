# CKA-experience

CKA的介绍以及和CKAD的一些区别网上资料很多，就不赘述了。
总结一下备考的一些经验，有些资料可能会稍有过时，但是仍不失为好的学习材料：

## 学习路径

从零开始学习K8S的路径建议：https://github.com/caicloud/kube-ladder

官网文档当然是考试最权威的参考资料，但是其文档组织不是安装由易到难的顺序组织的，显得比较混乱。
上面这个路径图是从易到难的一个概要，也可以作为检验自己k8s知识体系的参考。

## 官方大纲

官网考试大纲 ： https://github.com/cncf/curriculum
CKA和CKAD的大纲会公布在上面的repo里，可以看到CKA有不同的版本对应不同的kubernetes版本，考试一般都是用的最新K8S版本。
练习时要注意自己练习版本的k8s是不是和考试用的版本一致。

## 官方大纲和官方文档的对照

根据官方大纲整理的官网文档对照链接集 ： https://github.com/walidshaari/Kubernetes-Certified-Administrator

这个是我自己参考最多的文档，我认为每一条都要理解并且考试时可以快速找到官方文档的位置。
一定要熟悉官方文档的方方面面，时间上实际基本不允许从目录里慢慢找到需要的文档，甚至搜索也会显得浪费时间。
最好办法就是熟悉文档在目录中的位置，需要时快速定位并且可以从中找到需要的部分，如yaml，配置，关键字段等等。

## API Object 练习

快速创建API Object练习 ： https://github.com/dgkanatsios/CKAD-exercises

以命令而非yaml的方式快速创建API object,对于考试中节省时间非常重要。
但是建议在快速创建好object以后，仍然在master上保存一份yaml，以便复查修改。

## kubeadm搭建Cluster练习

官方文档 ： https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/create-cluster-kubeadm/

程序开发者一般比较少接触到k8s集群搭建的内容，要更加注意。在考试中这部分占分值很高且都是大题（6到8分）

特别要了解 https://kubernetes.io/docs/reference/command-line-tools-reference/kubelet-tls-bootstrapping/  及这个节点（command-line）的其他子文档里有关组件的配置参数的一些内容。
因为TLS bootstrapping理解起来比较难，另参见https://mritd.me/2018/08/28/kubernetes-tls-bootstrapping-with-bootstrap-token/ 。

## 二进制k8s组件搭建Cluster练习

原版： https://github.com/kelseyhightower/kubernetes-the-hard-way

中文版： https://github.com/caicloud/kube-ladder/blob/master/tutorials/lab3-manual-installtion.md

用二进制文件从零开始搭建k8s集群，会有助于更深入理解组件的作用和相互关系。建议至少练习三边。
同时注意，熟练使用"systemctl status","journalctl" 等工具查看各个组件的日志并排错也是考试内容之一。


