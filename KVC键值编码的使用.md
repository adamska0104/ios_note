# KVC键值编码的使用 {#1212}

##1.模型转字典的例子

```
void test6() {
    XMGPerson *person = [[XMGPerson alloc] init];
    person.name = @"lurry";
    person.money = 21.21;
    
    NSDictionary *dict = [person dictionaryWithValuesForKeys:@[@"name", @"money"]];
    NSLog(@"%@", dict);
}
```





