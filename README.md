![图片](https://user-images.githubusercontent.com/9653509/151100812-192a7f5a-5443-44da-ae85-d8101e091e2a.png)

A Queue that additionally supports operations that wait for the queue to become non-empty when retrieving an element, and wait for space to become available in the queue when storing an element.
BlockingQueue methods come in four forms, with different ways of handling operations that cannot be satisfied immediately, but may be satisfied at some point in the future: one throws an exception, the second returns a special value (either null or false, depending on the operation), the third blocks the current thread indefinitely until the operation can succeed, and the fourth blocks for only a given maximum time limit before giving up. These methods are summarized in the following table:
Summary of BlockingQueue methods

          Throws exception
            Special value
             Blocks
              Times out
Insert
add(e)
offer(e)
put(e)
offer(e, time, unit)
Remove
remove()
poll()
take()
poll(time, unit)
Examine
element()
peek()
not applicable
not applicable
