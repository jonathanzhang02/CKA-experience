# CKA-experience

CKA的介绍以及和CKAD的一些区别网上资料很多，就不赘述了。
总结一下备考的一些经验，有些资料可能会稍有落后，但是仍不失为好的学习材料：

## 学习路径

从零开始学习K8S的路径建议：https://github.com/caicloud/kube-ladder

官网文档当然是考试最权威的参考资料，但是其文档组织不是安装由易到难的顺序组织的，显得比较混乱。
上面这个路径是从易到难的一个概要，也可以作为检验自己k8s知识体系的参考

## 官方大纲

官网考试大纲 ： https://github.com/cncf/curriculum
CKA和CKAD的大纲会公布在上面的repo里，可以看到CKA有不同的版本对应不同的kubernetes版本，考试一般都是用的最新K8S版本。

## 官方大纲和官方文档的对照

根据官方大纲整理的官网文档对照链接集 ： https://github.com/walidshaari/Kubernetes-Certified-Administrator

这个是我自己参考最多的文档，我认为每一条都要理解并且考试时可以快速找到官方文档的位置。
一定要熟悉官方文档的方方面面，时间上实际基本不允许从目录里慢慢找到需要的文档，甚至搜索也会显得浪费时间。
最好办法就是熟悉文档在目录中的位置，需要时快速定位并且可以从中找到需要的部分，如yaml，配置，关键字段等等。

## API Object 练习

CKAD练习 ： https://github.com/dgkanatsios/CKAD-exercises

## kubeadm搭建Cluster练习

官方文档 ： https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/create-cluster-kubeadm/

特别要了解 https://kubernetes.io/docs/reference/command-line-tools-reference/kubelet-tls-bootstrapping/  及这个节点（command-line）的其他子文档里有关组件的配置参数的一些内容

## 二进制k8s组件搭建Cluster练习

原版： https://github.com/kelseyhightower/kubernetes-the-hard-way

中文版： https://github.com/caicloud/kube-ladder/blob/master/tutorials/lab3-manual-installtion.md


