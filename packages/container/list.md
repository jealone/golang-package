# list包
> import “container/list”

## 概述
list包用于实现双向链表

## 目录

### 包文件

## 内容
> type Element struct
- Value interface{} 
- 链表中的节点,包含一个interface{}类型的可访问值Value

> func(\*Element) Next() \*Element
- 返回当前节点的下一个元素或者nil(尾节点)

> func (\*Element) Prev \*Element
- 返回当前节点的上一个元素或者nil(头节点)

> type List struct
- 表示一个双向链表，零值为一个空的双向链表

> func New() \*List
- 初始化并返回一个双向链表

> func (l \*List) Back() \*Element
- 返回链表中的尾节点或者nil

> func (l \*List) Front() \*Element
- 返回链表中的头节点或者nil

> func (\*List) Init
- 初始化链表或者清空链表

> func (l \*List) InsertAfter(v interface{}, mark \*Element) \*Element
- 在链表的mark节点后插入值为v的节点并且返回该节点地址,如果mark不是链表中的元素，链表将不会发生改变

> func (l \*List) InsertBefore(v interface{}, mark \*Element) \*Element
- 在链表的mark节点前插入值为v的节点并且返回该节点地址,如果mark不是链表中的元素，链表将不会发生改变

> func (l \*List) Len() int
- 返回链表的长度，因为链表中存了长度值，所以该操作的时间复杂度为O(1)

> func (l \*List) MoveAfter(e, mark \*Element)
- 将链表中的节点e,移动到节点mark之后，如果e,和mark是同一个节点，或者有节点不存在与链表中，则不发生变化

> func (l \*List) MoveBefore(e, mark \*Element)
- 将链表中的节点e,移动到节点mark之前，如果e,和mark是同一个节点，或者有节点不存在与链表中，则不发生变化

> func (l \*List) MoveToBack(e \*Element)
- 将链表中的节点e移动到链表尾部，如果e在链表中，则不发生变化

> func (l \*List) MoveToFront(e \*Element)
- 将链表中的节点e移动到链表头部，如果e在链表中，则不发生变化

> func (l \*List) PushBack(v interface{}) \*Element
- 生成一个以v为值的新节点，插入到链表尾部，并且返回该节点地址

> func (l \*List) PushBackList(other \*List)
- 将链表other复制一份插入到链表尾部

> func (l \*List) PushFront(v interface{}) \*Element
- 生成一个以v为值的新节点，插入到链表头部，并且返回该节点地址

> func (l \*List) PushFrontList(other \*List)
- 将链表other复制一份插入到链表头部

> func (l \*List) Remove(e \*Element) interface{}
- 当e为链表的一个节点时，删除该节点，并且返回该节点的值








