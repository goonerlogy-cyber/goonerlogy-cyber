<div align="center">

<img src="./assets/header.svg" width="100%" alt="JAFN — small software. interesting internals." />

### JAFN

<sub>**goonerlogy-cyber**</sub>

small tools · clear purpose · useful diffs

I like terminals you can rewind, networks you can inspect, background jobs that finish cleanly, and algorithm visualizers that make the hard parts obvious. Currently working through interesting edge cases in **Go** and **TypeScript**.

[repos](https://github.com/goonerlogy-cyber?tab=repositories) · [pull requests](https://github.com/pulls?q=is%3Apr+is%3Aclosed+author%3Agoonerlogy-cyber)

</div>

<br/>

## on the workbench

Six forks I maintain. The linked pull requests document the changes now merged in those forks and how they were tested.

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://github.com/goonerlogy-cyber/replay"><img src="./assets/replay.svg" width="100%" alt="replay — terminal recording and playback" /></a>
      <p>Rewind a terminal. Keep its screen state intact.<br/><a href="https://github.com/goonerlogy-cyber/replay/pull/1">Alternate-screen support ↗</a></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/goonerlogy-cyber/portgraph"><img src="./assets/portgraph.svg" width="100%" alt="portgraph — live network connections" /></a>
      <p>See what is listening, and which process owns it.<br/><a href="https://github.com/goonerlogy-cyber/portgraph/pull/1">IPv6 connection discovery ↗</a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://github.com/goonerlogy-cyber/gitpulse"><img src="./assets/gitpulse.svg" width="100%" alt="gitpulse — Git repository analytics" /></a>
      <p>Turn repository activity into scriptable data.<br/><a href="https://github.com/goonerlogy-cyber/gitpulse/pull/1">Versioned JSON reports ↗</a></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/goonerlogy-cyber/toil"><img src="./assets/toil.svg" width="100%" alt="toil — background job processing" /></a>
      <p>Make worker shutdown a little less exciting.<br/><a href="https://github.com/goonerlogy-cyber/toil/pull/1">Reliable job completion ↗</a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://github.com/goonerlogy-cyber/cipherdrop"><img src="./assets/cipherdrop.svg" width="100%" alt="cipherdrop — encrypted, one-time sharing" /></a>
      <p>One-time sharing that stays one-time under load.<br/><a href="https://github.com/goonerlogy-cyber/cipherdrop/pull/1">Atomic burn-after-read ↗</a></p>
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/goonerlogy-cyber/zkaudit"><img src="./assets/zkaudit.svg" width="100%" alt="zkaudit — plaintext-leak auditing for browser captures" /></a>
      <p>Keep secret input exact, including whitespace.<br/><a href="https://github.com/goonerlogy-cyber/zkaudit/pull/1">File and stdin input ↗</a></p>
    </td>
  </tr>
</table>

These projects began with [arshnah](https://github.com/arshnah). My work is documented in the linked PRs and merged into my forks. Original authorship and licenses stay intact.

<details>
<summary>under the hood — changes & verification</summary>

| Project | Change | Checked with |
| --- | --- | --- |
| [replay](https://github.com/goonerlogy-cyber/replay/pull/1) | Independent alternate-screen state and cursor restoration while seeking. | Byte-stream and seek regression tests; Linux race checks; Windows tests. |
| [portgraph](https://github.com/goonerlogy-cyber/portgraph/pull/1) | IPv6 TCP/UDP discovery, process ownership, and readable polling failures. | Live IPv6 socket tests; Linux race checks; Windows parser tests. |
| [gitpulse](https://github.com/goonerlogy-cyber/gitpulse/pull/1) | JSON reports with accurate file accounting across paths and tracked symlinks. | Linux and Windows tests, vet, and build. |
| [toil](https://github.com/goonerlogy-cyber/toil/pull/1) | Bounded worker completion and observable queue-request errors. | HTTP regression tests, crash simulations, and Linux race checks. |
| [cipherdrop](https://github.com/goonerlogy-cyber/cipherdrop/pull/1) | Single-reader burn drops and expiry validation. | Multi-process regression tests and HTTP concurrency smoke tests. |
| [zkaudit](https://github.com/goonerlogy-cyber/zkaudit/pull/1) | Exact file/stdin input and rejection of empty secret scans. | Linux and Windows tests, vet, build, and Linux race checks. |

These changes are merged in my forks, not upstream releases. Each linked PR records the details and validation limits.

</details>

---

<div align="center">

<small>small scope · reproducible bugs · useful diffs</small>

</div>
