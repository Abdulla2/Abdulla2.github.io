# Abdulla: Bits of Tech Bites

## The first article of tech bites what is this and what I am doing here

### Introduction

A very long title that should have a question mark at its end but it
doesn't because I don't have an answer I don't really what I am doing
here but I'd like to think that it's good for me; I thought of the
title of this article and blog while I am takinga shower thought to
myself if it came to you in the bath it's good idea thought that bites
is a good wordplay of bytes and serves a double meaning but the more I
think of it the more I see it's dumb but I need a title so I went with
it anyway.

I am a tech guy my day job is a developer and I liked technology since I
was littleI am a typical nerd in this area but my nerdiness isn't
satisfied, I know a lot(Or that how my self perception is) but I did
very little for example I always dreamt of gaining new experiences
everyday and share it through a blog/vlog, I wanted always to make some
projects to learn tools and programming languages, to try new stuff here
and there, to tinker with open source projects and contribute to them,
but we're in the age of laziness and I must admit it I am lazy; I
finish my job sit on my couch and do nothing maybe pour a lot of time
into social media or just spend a whole night drowning in loop of
endless videos on youtube about nothing maybe interesting stuff and
maybe even not interesting.

So here I am making a commitment to write here every day -no promises
though- about tech stuff and whatnot maybe we'll tinker around, Nothing
in this blog will be AI all is authentic human so you'll find it more
funky a little-or maybe a lot- unorganized and you might find that I
didn't readproof it and it may have some mistakes I apologize for all
of that.

### How this site is built, C++ and other things

As stated above I had the idea for this for so long, I always wanted to make a yet another static site generator first to use it to generate my site/blog. From the introduction above you probably gussed it I haven't made my static site generator yet so I first wrote part of this aritcle in HTML but then told myself why am I doing this this way and wrote markdown and generated the html with pandoc, as you know minimalism is the new shiny thing in tech.

Regardless I started making a static site generator in C++, you ask why C++ because I wanted to expand my  experience in it and made a simple todo list program in it, and thought it would be fun if my second program was a static site generator.

I was this time serious in making the static site generator but I broke my hand and didn't finish anything, My hand is now healed thanks for asking and I will return to it and when it's finished I will use it to publish this site.


### The state of the so called static site generator

When I started writing it, I thought it would be good to write a C++ container that represents a tree data structure, one of the other projects I dreamed about is writing most of the STL but since my design for the static site generator needed a tree and there's no tree in the standard library of C++ it looked more and more appealing so here I am stuck at making C++ tree iterator with segfaults here and there maybe tomorrow It will be finished and I will share it with you, One can only hope.

Thank you, If there is anyone reading this I'd be surprised I wrote this to blow some ideas and I have a lot more I wrote it for myself to serve as a motivation but if you are reading it kind reader I'd be very happy to contact me on my linkedin on my github page.


## Second blog 

Usually blogs have the latest entries and articles on top so you read the latest and most relevant content in the present moment; Despite this I oughted to continue upon the first blog/article for 2 reasons: first it is easier in the current format(As you read above it's all plain text converted to plain html which you can view at github.com/abdulla2/abdulla2.github.io) and I am lazy and didn't want to organize for each blog. Second The first article wasn't complete maybe I'll opt for a wiki style personal site instead of a blog, I still have ideas connected to what I wrote above so here we are in a mixture of a blog and a personal wiki.

### The state of the tree 

I mean of course C++ tree, I looked upon it yesterday and found that it wasn't building fixed the build issues and fixed a segfault but entered an infinite loop in the iterator I made; I swear I am not a bad developer but please notice that I was getting into C++ newely and I haven't used it much and I am trying to do this to understand it more; also I don't give much time for this it was merely a 20 minutes yesterday remembering and fixing the issue.

### C++ nullptr_t argument overloading 

I encounterd a problem yesterday that this snippet:

```C++

		Iter(Tree* node, Iter* parent = nullptr) : m_node{node}, m_curr_child(node->m_children.begin()), m_parent(parent)
```

crushed because I Intited the Iter node with null if it is the end() node I thought to myself I should be able to overload the first argument with null and I was true tried it and worked and confirmed it from the C++ reference, a happy moment because I thought to myself ok I get it; I get how you should treat those things in C++, so here you have it a happy little story.

I will stop here give the tree a fair amount of trial to fix today and maybe continue this afterward.

### One 20 minutes later

Ok still not working but figured out why; as usual with modern C++ it has to do with moving semantics lvalue rvalue and those things, turns out I am returning a new object after each usage of operator++, I think I need after one month of not using C++ to revise some of the advanced things a little bit.

I think that's all for today I am feeling a strong fever and I can't go on in anything.

Wish me luck.

## Third Day, I think?

So the fever continues today I am not sure if I would be able to write anything today but let's try.

### Future Projects and wishes to add to this blog

As mentioned earlier I had planned without doing for the most of my professional and non-professional life that I want to contribute to open source projects and here I will list my wishes for projects I want to contribute to:

* Every Text editor I passed by: Vim, Nvim, Helix, Kakoune, you name it every one of them got my interest all of them lack some feature here or there that is critical or I was lazy to learn it anyway and I am using Vs Code at my day job but for my side projects I use mostly nvim, So What are the features I want in all of them first true Bidirectional text support and Arabic letters support regardless of the terminal or frontend used this also feature/or bug fix would be a recurrent theme of something missing in most projects I mention here: Ladybird, Foot Terminal.

* Other important feature that is lacking in nvim is multicursor support, they have it on their plan and it's semi-supported via some extensions but I want it out of the box.

* All those and that doesn't mean I wouldn't still use Vs Code, You can't teach an old dog a new trick anyway!

* Other Projects that I want to contribute to every lua engine out there especially of course the luajit I think there will be a lot of learning from this project.

* The Lua dev community highly represents the xkcd meme that says something about how many standards or version of something are there and someone think to himself I will solve all this by creating this new version that deprecates them all and then after that you'll have n+1 versions for the same thing.

* When I read lua documents I felt that its designers put too much thought into it from the beginning(They didn't design it in 10 days to match a deadline and yes I am looking at you javascript). also of course the JIT version is a state of art and its developer is a master anonymos dev going by Mike; The idea of compiler theory and programming languages design eluded me for long and the source code of lua is tempting to try tinkering and improving and so on.

* My obsessions extends to every open source project I think I can(Even if in reality I might not be able to but then again we will never be sure unless I tried) contribute to this includes OSes: Zephyr, SerenityOS, maybe Linux also, Libraries: LVGL, and any open source program I think to myself it will be benefetical for me to try and study and contribute to it.

### End of day

Today my thoughts, ideas and writings weren't organized very noisy I think I will pass by them tommorrow and try to give them a good editing or maybe not, Thank you for reading either way my mysterious reader.


## Fourth Day or Just let's not count

Edit you can skip and parenthises.

After finishing the writing of yesterday I had somewhat of a power and will to go into the tree code and rewrote parts of it and fixed issues and the tree iterator worked, YAY, This should have been a section of celebration, I have 3 options either go on without celebrating, edit this and remove all this rant and add a proper introduction with explainatories or 3 don't edit and keep the rant and make also a section to rant more.

### Tree Rant Section

So to start off what was the issue in my implementation, many things, and I know this is now a recurring theme that I swear each time I am not incompetent developer, but what is a competent developer anyway? (This is a philosophical question to derail you from putting me under the microsocope).

* I dumbly thought that (And I really don't know why I thought that this puts me again in very bad shape where you'll think I don't know how operator overloading works in C++) the return of the operator is the side effect I needed of it so ++operator for an int class type let's say will look like this

```C++
int operator++()
{
    return (*this + 1);

}
```

You can see the flaw here.

After fixing it I remembered why in the first place I decided to write this tree class, This was because I thought to myself that it would be a good idea to save the directory of the input markdown structure as is to generate the output with the same structure.

It is the weekend now and we'll see if I get doing anything useful or not.

Stay safe.


