converemojitostr
================

 很多时候，如果文字中夹带表情，那么这些文字的处理就会出现问题，例如，如果一个用户的昵称带有表情，那么我怎么把这个昵称转换为拼音呢？
 在实际的开发中，我遇到了这个个问题，先是找到了 https://github.com/iamcal/php-emoji这个转换表情的类库，但发现这个类库不支持ios6后新增的表情。
 最后没办法了，我写了个抓取程序，把 http://punchdrunker.github.io/iOSEmoji/table_html/ios6/index.html中ios6后新增的表情抓取出来，并写了个新的类库https://github.com/newjueqi/converemojitostr，这个类库的作用就是把文字中夹带的表情替换为一个特殊的字符(默认是"#")。
