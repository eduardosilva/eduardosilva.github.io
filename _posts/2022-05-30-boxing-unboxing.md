---
title: "Boxing & Unboxing"
subtitle: "Understanding .Net Boxing and Unboxing resource" 
header:
  teaser: /assets/images/gallery/conscious-design-TMFAwDy269I-unsplash.jpg
tags:
  - dotnet
  - csharp
---

Boxing and Unboxing is a very common question in .Net interviews. A good knowledge on this topic might by the difference in a hiring process.

Another important thing worth mention is performance. Sometimes performance issues are caused by lack of knowledge about types, cast and memory. So let's see some basics statements about it.

{% capture fig_img %}
![VisualStudioImage]({{ "/assets/images/gallery/conscious-design-TMFAwDy269I-unsplash.jpg" | relative_url }})
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Photo by <a href="https://unsplash.com/es/@conscious_design" target="_blank">Conscious Design</a> on <a href="https://unsplash.com/" target="_blank">Unsplash</a>.</figcaption>
</figure>


## Heap and Stack

Heap and Stack are the memory types where .Net Framework uses to store items.

**Stack**

* It's self managed;
* Store value types and pointers to Reference Types;


**Heap**

* It's managed by Garbage collector (GC);
* Store Reference types;

> That is a simplification. Not always a value type is stored in the stack (i.e., value type as attributes/properties in a object). If you want to learn more and understand the exceptions about type and references location in memory I recommend [The Truth About Value Types](https://docs.microsoft.com/en-us/archive/blogs/ericlippert/the-truth-about-value-types).

Let's take an example:

```c#
public static void Main()
{
    var mko = 1;
    var nji = 2;
    var obj = new MyClass();
}
```

Running this code we can imagine the following memory allocation:

| Stack                 | Heap              |
| ---                   | ---               |
| (mko) 1               | -                 |
| (nji) 2               | -                 |
| (obj) (Reference)     | MyClass (Object)  |

Ok, that's the basic about heap and stack, now we can see about boxing and unboxing.

## Boxing and Unboxing

Boxing is the process of converting a value type to the object. It's happens in a implicit way; Unboxing on the other hand, extracts the value type from the object by explicit way.

```c#
// Boxing
var mko = 1;
object obj = mko;

// Unboxing
var nji = (int)obj;
```

Why is important understand stack and heap to understand boxing and unboxing? So, that's why:

| Stack                 | Heap              |
| ---                   | ---               |
| (mko) 1               | -                 |
| (obj) (Reference)     | 1                 |
| (nji) 1               | 1                 |

When we convert a value type in a object it is created a reference from the stack to the heap, from that point we have time costs to allocate a reference in the stack, allocate the heap and we have the value 1 in two points `mko` in the stack and `obj` in the heap.

## Conclusion

There are many other details about this topic but this is a short description about boxing, unboxing and how this could affect performance in your application.

That's it, have a good one!