# \#KVC键值编码的使用 {#1212}

\#\#模型转字典

\`\`\` objc

/\*\*

\* 把模型转成字典

\*/

void test6\(\) {

XMGPerson \*person = \[\[XMGPerson alloc\] init\];

person.name = @"lurry";

person.money = 21.21;

NSDictionary \*dict = \[person dictionaryWithValuesForKeys:@\[@"name", @"money"\]\];

NSLog\(@"%@", dict\);

}

\`\`\`

