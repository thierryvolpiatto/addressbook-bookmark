Addressbook-bookmark
====================

You can  [![Support via Gratipay](https://cdn.rawgit.com/gratipay/gratipay-badge/2.1.3/dist/gratipay.png)](https://gratipay.com/thierryvolpiatto) or [![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=thierry.volpiatto@gmail.com&lc=US&currency_code=EUR&bn=PP-DonationsBF:btn_donateCC_LG.gif:NonHosted) to help this project.

## Description

This is an addressbook for Emacs based on standard Emacs bookmarks.
It provide completion on contacts in `message-mode` buffers,
a special mode to display contacts with address, phone etc...
If you have installed [google-maps](http://julien.danjou.info/google-maps-el.html)
you can switch to google map based on address of your contact.
It is fully compatible with [helm](https://github.com/emacs-helm/helm)
See `helm-filtered-bookmarks` and turn on `helm-mode` to have [helm](https://github.com/emacs-helm/helm) completion in message buffers.

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

Find a contact:

If you use [helm](https://github.com/emacs-helm/helm):

M-x `helm-filtered-bookmarks`

Otherwise:

M-x `bookmark-bmenu-list`

