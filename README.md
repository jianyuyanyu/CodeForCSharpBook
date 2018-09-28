# 《C# 从现象到本质》代码

如果希望成为一个C# 高手，或者至少是合格的C# 程序员，应该懂些什么？《C#从现象到本质》（以下简称本书）试图回答这个问题。实际上，在本书问世之前，市面上已经有很多优秀的C# 书籍，例如著名的《CLR via C#》《C# in Depth》，本书也参考了其中一些章节，但加入了这两本书没有覆盖到的一些重要知识点。本书基于C# 7.0编写。 

一个合格的C# 程序员必须熟悉C# 最核心的语言特性。本书没有讲基础的C# 语法，例如if/else/switch/while等等，因为人人都会。本书重点强调的是引用类型和值类型的区别和联系、委托与事件、泛型、反射、GC、LINQ相关、DLR相关，等等。这些知识对一些人来说，可能在实际开发中从来没有用到（例如DLR），或者一直都在使用但不自知（例如LINQ中隐含了委托）；但是，对这些内容是否深入理解，是区分一个批量生产的C# 程序员与一个合格的C# 程序员的很好方法。也许，你会觉得这些东西太过细微，似乎是“死抠书本”，但正如著名C# 程序员老赵曾经说的，“您也会觉得这些太细节，真要追究起来似乎也大都不是必须的，无视这些照样可以写程序，做网站，赚工资，但是我不会满足于成为（包括招聘）这样的程序员，暂时也懒得解释掌握这些东西的益处和重要性”。我对此的理解就是“project is cheap, show me the essential”。每个面试者都自带了若干个项目，你的优势在何处呢？你如何显现出水平高人一等呢？本书使用了大量的篇幅讲解C# 的核心语言特性，力求做到有一定的深度，和快速入门的书籍区别开。本书对任何一个语言特性，例如委托，都尽力阐述它的底层实现大概是怎样的，引入它是为了解决什么问题，在它没有出现时，类似的问题又是如何解决的。 

一个合格的C# 程序员应该知道程序的本质是什么，程序是如何在操作系统上运行起来的。《CLR via C#》之所以著名，因为它是第一个用CLR的视角来分析C# 语言的书（请仔细体会书名）。CLR的功能、两步编译、IL、对象在内存上的分布，这些内容可能在平时开发上真的用不到，但当你处理性能优化时，就会发现它们非常有用。 一个合格的C# 程序员应该对C# 提供的各种数据结构心中有数。数据结构和算法可谓程序设计的两大支柱，而现在它们的重要性似乎越来越小了，这是因为我们有太多的库可以直接拿来使用，不需要自己去实现一个经典的数据结构。也许我们不需要做到像算法工程师那样，对各种复杂的树（例如红黑树）、图有深刻认识，但是，对常见的数据结构，包括线性表、链表、队列、栈、哈希表等等概念和操作时间复杂度，是任何程序员都应该掌握的。本书的第11章专门讨论C# 的常见数据结构，这是同类型书籍较为少见的话题。 

一个合格的C# 程序员应该了解什么是线程，以及如何使用C# 进行多线程编程。如果一个WPF程序在执行耗时较长的任务时，界面直接冻结，用户只能坐等，那么这个程序肯定不会令人满意。C# 提供了非常丰富的类库可方便快捷地实现多线程。如果你想了解更多关于线程和进程的基本概念，本书的深度并不够，你可以找任意一本操作系统方面的书去研究。当多个线程有机会操作同一个资源时，线程同步变得十分重要。此时，需要有一个机制令同一时间只有有限个线程可以操作一个资源。C# 使用不同种类的锁来实现它。思路主要有两种：第一种是把资源操作变为原子的，称为用户模式的锁；第二种是将资源和一个内核对象挂钩，线程操作资源时需要去请示内核对象，这称为内核模式的锁。显然，由于访问内核对象速度很慢，还可以将这两种思路综合起来得到混合模式的锁，以加强锁的性能。本书的最后一部分比较详细地讨论了多线程的基本概念、同步以及各种多线程的实现方式，以最新的async/await作为结尾。 

如果你已经了解了上面所说的全部内容，那么在小白程序员眼中，你可能已经是一个C# 高手了。但很显然，还有很多很多东西本书没有涉及，例如设计模式、持续集成、测试、数据库访问、性能优化，等等。C# 程序员可以只会拖拖控件就能找到工作，也可以手握利剑解决别人解决不了的问题。我相信每个人都希望成为后者那样的类型，通过自己的努力，进入更好的公司，接触到更具有挑战性的项目，与更厉害的程序员共事。希望本书可以在你学习C# 的过程中，对你有所帮助。 


