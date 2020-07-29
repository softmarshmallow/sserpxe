# sserpxe
an express logic container, data access layer, clean and maintanable pattern




## How it is now.
prisma 
```typescript

const posts = await prisma.post.findMany({
  where: {
    title: {
      contains: "Hello",
    },
  },
});

```


## How it is with sserpxe
with prisma 
```typescript

const posts = await dals.posts.filterTitle({contains: "Hello"}).sort().fetchMany()

```

with sequlize
```

```