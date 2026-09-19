Question2Answer
-----------------------------

[Question2Answer][Q2A] (Q2A) is a popular free open source Q&A platform for PHP/MySQL, used by over 20,898 [sites] in 40 languages.

**This is a modified version of Question2Answer, not an official release.** See
[Modifications](#modifications) for what was changed and when.

**Note:** if you're using Q2A directly from git, make sure to use the master branch as that is the latest stable version. Or download an official release from the [Q2A website][Q2A].

Q2A is highly customisable with many awesome features:

- Asking and answering questions (duh!)
- Voting, comments, best answer selection, follow-on and closed questions.
- Complete user management including points-based reputation management.
- Create experts, editors, moderators and admins.
- Fast integrated search engine, plus checking for similar questions when asking.
- Categories (up to 4 levels deep) and/or tagging.
- Easy styling with CSS themes.
- Supports translation into any language.
- Custom sidebar, widgets, pages and links.
- SEO features such as neat URLs, microformats and XML Sitemaps.
- RSS, email notifications and personal news feeds.
- User avatars (or Gravatar) and custom fields.
- Private messages and public wall posts.
- Log in via Facebook or others (using plugins).
- Out-of-the-box WordPress 3+ integration.
- Out-of-the-box Joomla! 3.0+ integration (in conjunction with a Joomla! extension).
- Custom single sign-on support for other sites.
- PHP/MySQL scalable to millions of users and posts.
- Safe from XSS, CSRF and SQL injection attacks.
- Beat spam with captchas, rate-limiting, moderation and/or flagging.
- Block users, IP addresses, and censor words

Q2A also features an extensive plugin system:

- Modify the HTML output for a page with *layers*.
- Add custom pages to a Q2A site with *page modules*.
- Add extra content in various places with *widget modules*.
- Allow login via an external identity provider such as Facebook with *login modules*.
- Integrate WYSIWYG or other text editors with *editor/viewer modules*.
- Do something when certain actions take place with *event modules*.
- Validate and/or modify many types of user input with *filter modules*.
- Implement a custom search engine with *search modules*.
- Add extra spam protection with *captcha modules*.
- Extend many core Q2A functions using *function overrides*.


----------


All development is now taking place through GitHub. The collaborative development process is being managed by [Scott Vivian][1]. (Note that official releases are still distributed via the [Q2A website][Q2A].) See also:

- The [Q2A docs][2] for how to get started installing and using Q2A.
- The [Changelog][3] for what's new in each version.
- The [contributing file][4] for more information on how to get involved.


Thanks and enjoy!

Gideon & Scott


----------


Modifications
-----------------------------

This fork is a modified version of Question2Answer and is not an official Q2A
release. Modifications relative to upstream Q2A 1.8.8:

- **2026-09-19** - updated the bundled PHPMailer (6.6.3 to 6.12.0) and htmLawed
  (1.2.5 to 1.2.15.1), and adjusted `qa_sanitize_html_hook_tag()` for htmLawed's
  changed closing-tag convention; removed the end-of-life PHPMailer 5.2.28 along
  with the deprecated `qa-class.phpmailer.php` and `qa-class.smtp.php` shims;
  modernised the code for PHP 8 and raised the enforced minimum to PHP 7.1;
  aligned the source licence notices with the GPL v3 `LICENSE` file.

Official, unmodified releases are available from the [Q2A website][Q2A].


----------


License
-----------------------------

Question2Answer is free software released under the [GNU General Public License v3][license]
(or, at your option, any later version). The full licence text is in the `LICENSE` file.

Some bundled third-party components keep their own licences, which are unchanged:

- `qa-include/vendor/PHPMailer6` - LGPL v2.1.
- `qa-include/vendor/htmLawed.php` - dual licensed under LGPL v3 and GPL v2+.
- `qa-plugin/wysiwyg-editor/ckeditor` - see `qa-plugin/wysiwyg-editor/ckeditor/LICENSE.md`.
- `qa-plugin/recaptcha-captcha/recaptchalib.php` - MIT licence (see the header in that file).


[Q2A]: http://www.question2answer.org/
[1]: http://www.question2answer.org/qa/user/Scott
[2]: https://docs.question2answer.org/
[3]: https://docs.question2answer.org/install/versions/
[4]: https://github.com/q2a/question2answer/blob/master/CONTRIBUTING.md
[releases]: https://github.com/q2a/question2answer/releases
[sites]: http://www.question2answer.org/sites.php
[license]: https://www.gnu.org/licenses/gpl-3.0.html
