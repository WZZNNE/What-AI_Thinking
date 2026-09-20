# 新增作品 / Adding a piece

让收藏慢慢长大，每次只需照顾一个新文件夹和首页的一条介绍。

Let the collection grow one folder and one catalog entry at a time.

## 1. 建立文件夹 / Create a folder

放在 `projects/YYYY-MM-DD-short-name/` 下。日期使用作品首次加入收藏的日期，名称保持简短；后续修改继续留在同一目录。

Use `projects/YYYY-MM-DD-short-name/`. The date is when the piece first joins the collection. Keep the name short and make later revisions in the same folder.

每件作品包含自己的 `README.md` 和运行或阅读所需的文件。不同作品不必使用相同技术。

Each piece includes its own `README.md` and the files needed to run or read it. Different pieces may use different tools and formats.

## 2. 写双语项目介绍 / Write a bilingual introduction

项目 README 至少写清：作品是什么、如何打开、包含哪些内容、哪些部分实际检查过。中文与英文相邻排列；作品正文可以保留原始语言，并注明语言。

The project README should explain what it is, how to open it, what it contains, and what was actually checked. Place Chinese and English alongside each other. The work itself may keep its original language; identify that language in the introduction.

使用相对路径连接项目文件，并保留返回首页的链接：

Use relative paths for project files and include a link back to the main catalog:

```markdown
[← 返回收藏目录 / Back to the collection](../../README.md)
```

## 3. 在首页添加条目 / Add a catalog entry

在根目录 `README.md` 的“作品收藏 / The collection”部分末尾追加条目，编号顺延。写上日期、形式、一小段中英文简介，以及指向项目文件夹的链接。

Append an entry at the end of “作品收藏 / The collection” in the root `README.md`, using the next number. Include the date, medium, a short introduction in both languages, and a link to the project folder.

```markdown
### 002 · 中文作品名 / English title

**YYYY-MM-DD · 中文形式 / Medium in English**

一小段中文简介。

A short introduction in English.

**[进入项目 / Explore the project →](projects/YYYY-MM-DD-short-name/)**
```

## 4. 收进同一份收藏 / Keep the collection together

完成的作品都保留在 `main` 的独立文件夹中。需要时可用临时分支制作或修改，完成后合并回来；不使用永久分支分别存放每件作品。

Finished pieces belong in separate folders on `main`. Temporary branches can be used to create or revise a piece and merged back when ready. Do not use permanent branches as separate storage for each work.
