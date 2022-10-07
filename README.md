# GameMaker-wheat_ptr

你可以使用两种方式来创建一个 小麦指针：

    p = make_wheat_ptr(); // 使用该方式创建的 wheat_ptr 不需要手动释放内存
    p = new wheat_ptr(); // 使用该方式创建的 wheat_ptr 需要手动 delete 来释放内存
  
    // 当你在写下这两行时，鼠标悬停在 make_wheat_ptr() 或 wheat_ptr() 上，能看到我写的注释，你可以根据这些注释来进行初始化工作
  
一些成员函数：

    p.point() // 指向目标
    p.value() // 获取值，若获取失败会返回 undefined
    p.set()   // 设定值到指向的变量，成功返回 true，失败返回 false
    p.get()   // 返回该 wheat_ptr 所指向的目标相关的数据，返回结果也是一个结构体，但是并非用 new 创建，所以不需要手动释放内存
    p.swap()  // 互换两个 wheat_ptr 所指向的目标（不会对被指向的变量的值产生影响），成功返回 true，失败返回 false
  
    // 详细参数请将鼠标放在对应的函数上查看注释
  
