# NOTES
my notes

python "D:\documents\ai\python\my-first-conda-project\_read to me args (with read time and csv stats) 1.py" "

commenter:drakeredwind01

suggest removing `needs-triage` `needs-sig` and adding `triage/accepted`, `sig-network`, and `sig-security`

## O3DE Network SIG - Issue Triage Guide
https://github.com/o3de/o3de/issues?q=is%3Aissue%20is%3Aopen%20label%3Aneeds-triage%20-label%3Asig%2Fnetwork%20%20--label%3Asig%2Fbuild%20--label%3Asig%2Fbuild%20%20--sig%2Fgraphics-audio%20%20--sig%2Fcontent

1. Open issues with `needs-sig` label: https://github.com/o3de/o3de/issues?q=is%3Aissue+is%3Aopen+label%3Aneeds-sig
   1. `OLD` 
   2. `NEW` 
2. Main O3DE repository: 
   1. `OLD` https://github.com/o3de/o3de/issues?q=is%3Aissue+is%3Aopen+label%3Aneeds-triage+label%3Asig%2Fnetwork
   2. `NEW` `works` https://github.com/o3de/o3de/issues?q=is%3Aissue+is%3Aopen+label%3Aneeds-triage+-label%3Asig%2Fnetwork++--label%3Asig%2Fbuild+--label%3Asig%2Fbuild+
>     altered is:issue is:open label:needs-triage label:sig/network
>      to     is:issue is:open label:needs-triage -label:sig/network  -label:sig/build -label:sig/build  
3. Multiplayer Sample: https://github.com/o3de/o3de-multiplayersample/labels/needs-triage
   1. `OLD` 
   2. `NEW` 
4. NetSoak Test: https://github.com/o3de/o3de-netsoaktest/issues
   1. `OLD` 
   2. `NEW` 
5. [Multiplayer template](https://github.com/o3de/o3de-extras/tree/development/Templates/Multiplayer) issues in: 
   1. `OLD` issues in: https://github.com/o3de/o3de-extras/labels/sig%2Fnetwork
   2. `NEW` issues in: https://github.com/o3de/o3de-extras/issues?q=is%3Aopen+label%3Asig%2Fnetwork+++-label%3Asig%2Fnetwork+-label%3Asig%2Fcore+-label%3Asig%2Fbuild+-label%3Asig%2Fsimulation+-label%3Asig%2Frelease+-label%3Asig%2Fgraphics-audio+-label%3Asig%2Fplatform+
>     altered is:open label:sig/network  -label:sig/network
>      to      is:open label:sig/network   -label:sig/network -label:sig/core -label:sig/build -label:sig/simulation -label:sig/release -label:sig/graphics-audio -label:sig/platform  





## O3DE sig-security - Issue Triage Guide
https://github.com/o3de/sig-security/blob/main/TRIAGE_GUIDE.md

* O3DE issues to triage for SIG:
    * https://github.com/o3de/o3de/issues?q=is%3Aissue+is%3Aopen+label%3Aneeds-triage+label%3Asig%2Fsecurity
    * `works`https://github.com/o3de/o3de/issues?q=is%3Aissue+is%3Aopen+label%3Aneeds-triage+-label%3Asig%2Fsecurity+-label%3Asig%2Fbuild+-label%3Asig%2Fcontent+-label%3Asig%2Fcore+-label%3Asig%2Fdocs-community+-label%3Asig%2Fnetwork+-label%3Asig%2Fplatform+-label%3Asig%2Fgraphics-audio+-label%3Asig%2Frelease+-label%3Asig%2Fsimulation+-label%3Asig%2Ftesting+-label%3Asig%2Fui-ux+-label%3Asig%2FTAC%2FTSC+-label%3Asig%2Fmobile+
* O3DE known security issues: 
    * https://github.com/o3de/o3de/issues?q=is%3Aissue+is%3Aopen+label%3Akind%2Fsecurity
    * `works`https://github.com/o3de/o3de/issues?q=is%3Aissue+is%3Aopen+label%3Akind%2Fsecurity+-label%3Atriage%2Faccepted+-kind%3Akind%2Fsecurity
* Dependabot alerts to check (link only accessible to SIG-Security maintainers): 
  <br>`broken` https://github.com/o3de/o3de/security/dependabot
    * For new alerts, create new GitHub issues against [O3DE](https://github.com/o3de/o3de) and tag with `kind\security` label for tracking.
    * **WARNING**: Since the O3DE _python/requirements.txt_ file includes hashes, Dependabot-generated PRs against this file should be **manually tested** against a clean `/python` folder (that is, no `/runtime` child dir) **prior to merging** in order to suss out any issues with hashing transitive dependencies.








| sig-{name}           | responsible for                        |
|----------------------|----------------------------------------|
| `sig-build`          | coding errors,                         |
| `sig-content`        |                                        |
| `sig-core`           |                                        |
| `sig-docs-community` | problems with the documentation        |
| `sig-network`        | anything to do with multiplayer sample |
| `sig-platform`       | not working on different platforms/OSs |
| `sig-graphics-audio` | terrain,coloring, and sound issues     |
| `sig-release`        |                                        |
| `sig-security`       | security issues                        |
| `sig-simulation`     |                                        |
| `sig-testing`        |                                        |
| `sig-ui-ux`          | GUI, windows layout                    |
| `sig-TAC/TSC`        |                                        |
| `sig-mobile`         | phone, hand held, etc.                 |

[Gitflow workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)

| branch  | how to incorperate | notes                                                                |
|---------|--------------------|----------------------------------------------------------------------|
| bugfix: | [bugfix/]          | problem that should be fixed that doesn't add any new functionality  |
| Feature | [feature/]         | an attribute or characteristic that adds value to the product.       |
| Release | [release/]         | where the maintainers believe the software is worth trying and using |
| Hotfix  | [hotfix/]          | should never use. needs to be added right away into production       |

a patch is a change to a piece of software


- [text Sizes](#text-Size-1)

> ## show and tell JT
> > - [ ]                         use ``[title](link)`` 




> ## O3DE
> [TRIAGE_GUIDE.md](https://github.com/o3de/sig-network/blob/main/TRIAGE_GUIDE.md)
> > ### for triage notes
> > ask:
> > > should we add tag:
> > > > [needs-priority](https://github.com/o3de/o3de/labels/needs-priority)
> > > >
> > > > > Indicates a PR lacks a `priority/foo` label and requires one.
> > > >
> > > > [priority/critical](https://github.com/o3de/o3de/labels/priority%2Fcritical)
> > > >
> > > > > Critical priority. Must be actively worked on as someone's top priority right now.
> > > >
> > > > [priority/minor](https://github.com/o3de/o3de/labels/priority%2Fminor)
> > > >
> > > > > Lowest priority. Work that may be scheduled
> > > >
> > > > [priority/blocker](https://github.com/o3de/o3de/labels/priority%2Fblocker)
> > > >
> > > > > Highest priority. Must be actively worked on right now as it is blocking other work.
> > > >
> > > > [priority/major](https://github.com/o3de/o3de/labels/priority%2Fmajor)
> > > >
> > > > > Major priority. Work that should be handled after all blocking and critical work is done.
> > > >
> > > > [triage/needs-information](https://github.com/o3de/o3de/labels/triage%2Fneeds-information)
> > > > 
> > > > [status/needs-testing](https://github.com/o3de/o3de/labels/status%2Fneeds-testing)
> >
> > 
> > 
> > 
> > mention this in everything so that it is always seen and gets done
> > 
> > > [Give drakeredwind01 labeling permission #16108](https://github.com/o3de/o3de/issues/16108)
> > > 
> > > ["triage-complete" label #15877](https://github.com/o3de/o3de/issues/15877)
> > > 
> > > [Feature Request add "Feature Request" label #15876](https://github.com/o3de/o3de/issues/15876)
```
["triage-complete" label #15877](https://github.com/o3de/o3de/issues/15877)
```

## quetions to ask

just wondering
going to add feature "include build in window banner e.g. "O3DE 2.32 or Commit ID e5d4b63 (64-bit, windows) {other useful info} {project name}"
also have a copyable version in the about for the O3DE engine.


## Example:
> [how-to-GitHub-markdown](https://github.com/drakeredwind01/how-to-GitHub)
> 
> how-to-GitHub-markdown[^how-to-GitHub-markdown1]
> 
> 
[^how-to-GitHub-markdown1]:
    how-to-GitHub-markdown
    [how-to-GitHub-markdown](https://github.com/drakeredwind01/how-to-GitHub)
    [how-to-GitHub-markdown]
    

## JT
> go back to talking about xyntopia/pydoxtools
> 
> > making survival resources
> > 
> really need work
> 
> show sigma delta list
### contributed
> [Add "triage-complete" label #15877](https://github.com/o3de/o3de/issues/15877)
> 
> [Module Manager window pops-up when launching AutomatedTesting project with -rhi=Vulcan enabled #16028
](https://github.com/o3de/o3de/issues/16028)




## notes
> only ask don't suggest
> 
> make people notes on O3DE group
> 
> WIP (work in progress)
> 
> potential work
> 
> > mat bino in python group has a advertising group. tell him about my "ΑΣΩΓ" and see if they will hire me
> > 
> > retry arrow staffing for work
> > 
> > try technical staffing in san diego for work
> > 
> > tell them I only want short term projects
> > 
> > > gorila suit

## lookup
> hudeny

2023.08.31.10.52.48.346
> Bug Report - Monolithic Game Export created via Export Script does not work in Output folder #16632
> > Dependencies.xml missing


