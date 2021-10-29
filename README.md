### Linus Torvalds: A Lesson in Vigilance

> Mauro, SHUT THE F**K UP!

TODO Profile Picture

Linus Torvalds can be widely regarded as one of the most influential software engineer
of our times. His kernel is the heart for up to three-quarters of all public web servers[^1] and
runs every modern supercomputer since late 2017[^2]. His version control system is reportedly used
by upwards of 85% of all software developers[^3], including this GitHub repository. Most impressively,
both of these projects are completely free and open-source[^f1], developed by thousands of individual
contributors and companies[^4] around the globe. How is it possible for Torvalds to maintain and direct
arguably one of the most successful and important open-source project today?

Torvalds was born in Helsinki, Finland, on 28 December 1969. From as early as eleven years old, he could
be found programming a Commodore VIC-20 first in the high-level BASIC programming language and later moving
down to the raw 6502 CPUs machine code. Later again he would purchase a Sinclair QL where he developed his
own tools and games and even tinkered with the operating system (*foreshadowing?*).

It's interesting to compare his childhood to my own: I, too, began programming at eleven. Initially, I
fiddled around with the files of video games I owned[^f2] and used high-level game development software to
make my own with JavaScript. Over the next few years, I found myself programming in lower-level languages
such as C#, C++ and even Assembly. My reasoning for doing this was never entirely clear, but I would
consider both an interest in understanding how computers worked and trying to squeeze as much performance
out of them as possible as primary factors.

While Torvalds studied computer science at the University of Helsinki, he began development on what was
to become Linux, initially called Freax[^f3]. He announced it along with its source code on Minixs[^f4] IRC later
that year, looking for feedback and suggestions[^5]. At a similar time, he was introduced to
the GNU Project then Richard Stallman held a speech at Helsinki University of Technology. Torvalds was inspired enough to
eventually license his new kernel under the GNU General Purpose License in 1992. 18 years later, I would
also fall for Stallman's talking points and adopt the modern GNU GPLv3 as my go to open-source license.

Even before then, Torvalds was already using and supporting much of the GNU Projects work. The initial release
of Linux, aptly titled Linux 0.01, included GNU's Bash shell and recommended installing GNU software to
supplement the kernel for use as an actual operating system[^f5]. Clearly, Torvalds was not interested in
developing an entire operating system with the hundreds of required utility programs, but instead would
specialise in only the kernel and let GNU Project and similar provide userspace tools.

I respect Torvalds for having the discipline to draw a line in his projects scope and not fall victim to
feature creep. Additionally, I appreciate the difficultly in accepting other developers projects as either
dependencies or supporting them yourself when developing your own project[^f6]. I would consider this to be
one of open-sources core strengths: Permissive licensing makes it easy to depend on and support other
software without the hassle of copyright infringement and the propagation of closed-source software drivers.

Moving forward, Torvalds continued to work on his kernel with help from over one-hundred other contributors.
By 1994, Torvalds releases Linux 1.0 with full support for the GNU software environment GUI with XFree86[^f7].
Already, many distributions of Linux were being produced by various teams and companies. Slackware and Debian
are still well known today, while Red Hat and SUSE contribute greatly to the kernel and maintain their own
enterprise Linux distributions. Within an additional four years, Linux would come to support many processors
and would in turn be supported by many major companies such as IBM and Oracle. Clearly, by this time, Linux
was a well recognised and respected open-source project. Within the decade, Linux would grow to over two
million lines of code in length with over 250 individual and company contributors[^7] from a plethora of countries.
By 2011, it was reaching ten million lines of code and 1,200 contributors.

How did this happen? I thought collaboration was difficult and programmers were unsociable?[^f8] As stated before,
Torvalds licensed Linux as an open-source community project. As such, it used the open-source development model[^8].
While not a formal development methodology like we have studied, it describes a development process that tends to
emerge when large distributed teams work on a non-trivial codebase, much like most open-source projects.
Users submit bug reports and feature requests, participating developers contribute code to address these issues and
a select group of project maintainers review and accept contributed code before releasing a collection of
contributions as a stable patch or update.

TODO Diagram

It's important to note that this model lends itself nicely to tight incremental development loops, continuous
testing/integration and well maintainable code. These components by themselves can prove to be enough to keep
an open-source project from spiralling out of control or grinding to a halt in development hell. However, I
believe what held Linux together for all these years was Torvalds.

Torvalds has stated that Linux was never meant to specifically be an open-source project, but instead proved to
be the best way of working with other developers around the world.

> I did not start Linux as a collaborative project, I started it for myself. I needed the end result but I also
> enjoyed programming. I made it publicly available but I had no intention to use the open-source methodology,
> I just wanted to have comments on the work.

TODO Working together with thousands of contributors using mailing lists, vigilance

*Ted Johnson\
TCD 19335618*

[^f1]: There is some controversy surrounding closed-source device drivers being included in the Linux kernel.
[^f2]: This could be considered 'game modding', but I wasn't nearly skilled enough to produce anything interesting!
[^f3]: It was actually an administrator for a FTP server being used that changed the file names without consulting Torvalds.
[^f4]: At this time, the Linux kernel ['resembles it somewhat'][^5]. It wouldn't be long until Torvalds would enter a now famous flame war with Minix developer Andrew Tanenbaum over the kernel design differences between the projects.
[^f5]: See the humorous misquote of Stallman and his response regarding using GNU software with the Linux kernel [here](https://www.gnu.org/gnu/incorrect-quotation).
[^f6]: Not Invented Here (NIH) syndrome.
[^f7]: XFree86 would go on to reform as the X.Org Foundations in 2004, which still maintains the X server software generally used with Linux today.
[^f8]: This is a joke. Well, mostly a joke.

[^1]: https://w3techs.com/technologies/details/os-linux
[^2]: https://www.top500.org/statistics/details/osfam/1
[^3]: https://insights.stackoverflow.com/survey/2018
[^4]: https://www.linuxfoundation.org/tools/participating-in-open-source-communities
[^5]: https://groups.google.com/g/comp.os.minix/c/dlNtH7RRrGA/m/SwRavCzVE7gJ
[^6]: https://firstmonday.org/ojs/index.php/fm/article/download/1151/1071
[^7]: https://www.ted.com/talks/linus_torvalds_the_mind_behind_linux
[^8]: https://www.ibrahimatlinux.com/uploads/6/3/9/7/6397792/00.pdf
