Jekyll.vim
==========

jekyll.vim:  Blogging from the command line should not be tedious.

This script is intended to automate the process of creating and editing [Jekyll](http://jekyllrb.com/) blog posts from within [vim](http://www.vim.org/).

Introduction
============

Install using VimPlug

`Plug 'pixelatedstack/jekyll.vim'`

Set the path to your Jekyll Blog in your vimrc:

    let g:jekyll_path = "/path/to/jekyll/blog"

The default post suffix is "markdown". 

Example:
    let g:jekyll_post_suffix = "textile"

You may also want to ad a few mappings to stream line the behavior:

    map <Leader>jb  :JekyllBuild<CR>
    map <Leader>jn  :JekyllPost<CR>
    map <Leader>jl  :JekyllList<CR>


By default all posts are created as drafts (published: false in the YAML), to publish that post simply delete that line.

Commands
========

Build Jekyll site:

    :JekyllBuild

List Jekyll posts:

    :JekyllList

Create a new Jekyll Post:

    :JekyllPost

LICENSE
=======

License: Same terms as Vim itself (see [license](http://vimdoc.sourceforge.net/htmldoc/uganda.html#license))

:-)
