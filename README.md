# Anime Character Recognizer

An app for you to look up an anime character and the series which her/him belongs to.

## Log

### Day 1

In a boring weekend evening after the end of my course in university, I coincidentally read an interesting article from [freedomofkeima's blog - Image Recognition for Anime characters using Deep Learning](https://freedomofkeima.com/blog/posts/flag-15-image-recognition-for-anime-characters).

Well, I'm a newbie in ML and reading formal theories and other complicated stuffs last month really stressed me out. Hence, I guess this little app could be a toy project for me to learn ML in a different and fun (yeah I'm really into anime) approach besides my formal learning path.

The basic features I'm planning for this app to have are:

* Detects anime faces in an image

* Retrieve detail info about the characters whose faces in the image

That's it.

In short, this is the blog about what I learned, read and searched for to complete (hope so, LOL) this project. 

Enough chitchat! Time is candy!

Now, after 15 mins of blog reading, we can see Iskandar's (writer of *Freedomofkeima*) approach consisted of 3 steps:

```
1.Utilize lbpcascade_animeface to recognize character face from each images
2.Resize each images to 96 x 96 pixels
3.Split images into training & test before creating the final model
```

Stucked right in the first step, so what is **lbpcascade** he was talking about!??
#### What is LBP Classifier
According to [pyimagesearch](https://www.pyimagesearch.com/2015/12/07/local-binary-patterns-with-python-opencv/)

> LBPs ... compute a local representation of texture. This local representation is constructed by comparing each pixel with its surrounding neighborhood of pixels.


Back to where we paused, Iskandar project suggests we use an LBP cascade from [Nagadomi-AnimeFace](http://anime.udp.jp/data/lbpcascade_animeface.xml)