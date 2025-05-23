You can obtain development builds directly from GitHub. Every time the CI server performs automated tests on the code, it also creates an apk file that you can try. **These builds are not meant for daily use.** As they are debug builds, they are significantly slower/laggier and they may crash when detecting some (usually unproblematic) programming errors, instead of ignoring them like release builds. Use them for testing only.

- Open a branch to view the commits, click the checkmark (or cross) icon and select any of the tests:
{% include image.html
   width="250"
   alt="An image showing completed checks on a branch, with an arrow pointing to the Details link."
   loc="/assets/images/contribute"
   file="testbuild1.png"
%}
- Choose `Summary`:  
{% include image.html
   width="250"
   alt="An image with an arrow pointing to the Summary link for checks on a branch."
   loc="/assets/images/contribute"
   file="testbuild2.png"
%}
- Scroll down and download the artifact:  
{% include image.html
   width="250"
   alt="An image with an arrow pointing to a test build generated by the CI server."
   loc="/assets/images/contribute"
   file="testbuild3.png"
%}
