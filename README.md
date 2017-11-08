Addressbook-bookmark
====================

You can [![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=thierry.volpiatto@gmail.com&lc=US&currency_code=EUR&bn=PP-DonationsBF:btn_donateCC_LG.gif:NonHosted) to help this project.

## Description

This is an addressbook for Emacs based on standard Emacs bookmarks.
It provide completion on contacts in `message-mode` buffers,
a special mode to display contacts with address, phone etc...
If you have installed [google-maps](http://julien.danjou.info/google-maps-el.html)
you can switch to google map based on address of your contact.
It is fully compatible with [helm](https://github.com/emacs-helm/helm), you will need [helm-addressbook](https://github.com/emacs-helm/helm-addressbook)
extension.
To have [helm](https://github.com/emacs-helm/helm) completion in message buffers turn on `helm-mode`.
You don't need helm as dependency but for a better experience you are adviced to use it.

## Installation

Add addressbook-bookmark.el to your `load-path` and add to your init file:

     (require 'addressbook-bookmark)

If you want completion in message buffer:

     (eval-after-load "addressbook-bookmark.el" (addressbook-turn-on-mail-completion))

If you want [helm](https://github.com/emacs-helm/helm) completion on contacts while completing from your message buffer turn on `helm-mode`.

## Usage

Add some contacts to bookmark:

M-x `addressbook-bookmark-set`

Add a contact from gnus summary:

M-x `addressbook-gnus-sum-bookmark`

Add a contact from a mu4e view buffer:

M-x `addressbook-mu4e-bookmark`

Find a contact:

If you use [helm-addressbook](https://github.com/emacs-helm/helm-addressbook)

M-x `helm-addressbook-bookmarks`

Otherwise:

M-x `bookmark-bmenu-list`

