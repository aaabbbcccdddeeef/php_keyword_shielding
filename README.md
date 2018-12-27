# keyword_shielding
敏感词过滤，基于DFA敏感词过滤算法，忽略所有(空格,`,~,#,$,^,&amp;,*,_),并且自动将敏感词更换为*

 * 敏感词过滤，基于DFA敏感词过滤算法，大字典的时候比较高效。
 * 使用只需要将本文件引入，然后再调用shildDirtyWords::findAndHideKeyWords($testWords)即可
 * 如果使用shildDirtyWords::findAndHideKeyWords($testWords)来屏蔽，会有比较好的屏蔽效果，
 * 这个是对字典的补充，忽略了一些无意义的词，但也可能造成语义的一点曲解。注意斟酌使用
 * 需要及时更新敏感词字典，敏感词字典在/Resources/BadWord.txt
