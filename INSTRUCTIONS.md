# asciidoctor Test - Selective Files Test Result

Ctrl + click [test results](https://jhauga.github.io/htmlpreview.github.com/?https://github.com/CHANGE_USER/CHANGE_REPO/blob/main/index.html).

The files used for the test were either selected becuase they had elements the pull request addresses, or selected at random.
Expand below to show test files:
<details>
 <summary>Show Files Tested</summary>
  
   - git-lfs-clean.adoc
   - git-lfs-clone.adoc
   - git-lfs-faq.adoc
   - git-lfs-filter-process.adoc
   - git-lfs-lock.adoc
   - git-lfs-merge-driver.adoc
   - git-lfs-pointer.adoc
   - git-lfs-post-checkout.adoc
   - git-lfs-post-merge.adoc
   - git-lfs-pull.adoc
   - README.adoc
   - asciidoctor.adoc
   - basic.adoc
   - convert-files.adoc
   - docbook-xml.adoc
   - features.adoc
   - index.adoc
   - manpage.adoc
   - mdbasics.adoc
   - options.adoc
   - output-file.adoc

</details>

## Test Procedure - Condensed:
1. Set configuration and ready test elements.
2. Pending on configuration Either:
   - Clone source (*asciidoctor*) and pull (*jhauga*) asciidoctor repo.
   - Copied and used local version of asciidoctor asciidoctor tool and jhauga asciidoctor
3. Start test function configuring function for source or pull.
4. Set a start and end time for each build with asciidoctor, pushing start and end to two separate arrays.
5. In ` run_command() ` sub-function call asciidoctor first utilizing prior configurations to build using source or pull asciidoctor and calculate build time(s).
   - Additional marker here cause this is where asciidoctor is called and timed.
6. Determine difference after all files built second in `runc_command() sub-function.
7. Call ` run_command() ` sub-function.
8. Determine if there is a difference, checking empty files and count number of differences.
9. Call ` run_test() ` function with source or pull, reconfigure and call ` run_test() ` again.
10. Make support html elements for difference output and dropdown menus.
11. Compare total fies built to files with differences, outputting results to supporting text file.
12. Calculate stats for build times, outputting results to supporting text file.
13. Make remaining support html elements and clean files and directories.
