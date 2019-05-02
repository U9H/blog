+++
title = "2019-05-02 — Weekly Update"
date = 2019-05-02T05:19:06-06:00
draft = false
description = "What I'm working on this week"

[taxonomies]
authors = ["Alexander Lozada"]
categories = ["news"]
+++

# Weekly Update

It's been a while since I've posted much, but I've been doing a lot lately. To stay motivated and aware of progress, I'm starting to log my progress weekly. Here, I'll record what I've worked on for the week, and what I hope to accomplish soon.

## Week of 2910-04-29

### rust.audio

This week, [rust.audio](//rust.audio) was (sort of) launched. There's still a fair amount of work to be done, but as of now it's structurally sound.

This site was made for and with our team ([rust-dsp on GitHub](//github.com/rust-dsp/)), and hopes to become a center for audio programming resources in the Rust programming language.

As a disclaimer, this site does not have any official affiliation with the `RustAudio` people on GitHub.

Others have also started work on an `lv2` implementation in Rust. Well, there's actually a few already — but two authors are combining their efforts.

### U9H Newsletter

The U9H Newsletter Zola theme has been updated a bit to provide a better reading experience for desktop users. Expect more improvements in the future as the theme is still pretty rough.

### Amethyst

I haven't been as active in the Amethyst community this week, but contributors are continuing to work towards [Rendy](//github.com/omni-viral/rendy/) integration, not to mention the exciting [10k Grant provided by Mozilla](//amethyst.rs/blog/moss-grant-announce/).

### Side Projects
I've been working on a small crate for generating random data from arbitrary data structures. While probably not very idiomatic, I used the opportunity to learn more about Rust's type system, as well as iterators. In fact, I found implementing the `Iterator` trait super useful for my Generator. With it, I can perform lots of nice operations on the dataset before retrieving random values. For example, take the following.

```rs
// this is sort of psuedocode
let gen = Generator::<SomeType>::new();

// return 5 random values after filtering
gen.filter(|x| x.some_field).get(5)
```

The original motivation was to create a more in-depth [Fake Clients](//fakeclients.com/)-esqe site. I'd like to be able to generate situations, previous styles, branding, and other attributes procedurally.

## Future

I'm going to continue a fair bit of web dev for the moment, as well as work on my clients application. The index page of the blog especially needs attention.

I'd also like to experiment with making a simple rhythm game in Amethyst if time permits. 