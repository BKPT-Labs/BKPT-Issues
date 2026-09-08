# BKPT Issues

Bug reports, feature requests and questions for the BKPT Labs tools, in one
place. If something in a BKPT product does not work the way you expected,
this is where to tell us. Every report is read.

## What this covers

| Product | Where you use it |
| --- | --- |
| [BKPT Debug](https://marketplace.visualstudio.com/items?itemName=BKPT.bkpt-debug) | VS Code extension: debugging, Fault Analyzer, PC sampling, ETM history, live watch, peripheral registers, ITM console |
| [BKPT ViewAlyzer - Embedded Trace](https://marketplace.visualstudio.com/items?itemName=BKPT.bkpt-viewalyzer) | VS Code extension: recording and viewing RTOS and event traces |
| ViewAlyzer desktop and `viewalyzer-cli` | The desktop trace viewer and the headless capture and query tool |
| ViewAlyzer Recorder | The firmware-side recorder for Zephyr, FreeRTOS and baremetal |
| viewalyzer-sdk | The Python package that wraps the CLI |

Product pages and documentation live at [bkptlabs.com](https://bkptlabs.com).

## Before you open an issue

1. Search the [existing issues](https://github.com/BKPT-Labs/BKPT-Issues/issues).
   If yours is already there, add a comment or a thumbs up instead of a new
   report. It helps us rank what to fix first.
2. Check the docs for the feature at [bkptlabs.com/docs](https://bkptlabs.com/docs/).
   Many "it does not work" cases are a missing wire, a probe the core does
   not support, or firmware that does not match the ELF. Both extensions try
   to say so on screen; if they did not, that is worth a report on its own.
3. Update to the latest release of the extension or tool.

## Reporting a bug

Open a [new issue](https://github.com/BKPT-Labs/BKPT-Issues/issues/new) and
include as much of this as you can:

- **Product and version.** In VS Code, hover the extension in the Extensions
  view. For the desktop app and CLI, run `viewalyzer-cli --version`.
- **Host.** Windows, macOS or Linux, and the version.
- **Target.** Board or MCU part number, and the RTOS if any.
- **Probe.** ST-LINK or J-Link, the probe firmware version if you know it,
  and whether SWO or trace pins are wired.
- **What you did, what you expected, what happened.** Short numbered steps
  are ideal.
- **Evidence.** A screenshot of the panel, and the relevant log:
  - BKPT Debug: the **BKPT Debug** channel in the VS Code Output panel.
  - ViewAlyzer for VS Code: run **ViewAlyzer: Check Setup Health**, click
    **Copy report** and paste the result.
  - A `.vadb` recording that shows the problem, if you can share it.

Please strip anything confidential from logs and recordings before you attach
them. Do not post license keys.

## Requesting a feature

Open a [new issue](https://github.com/BKPT-Labs/BKPT-Issues/issues/new) and
describe the problem you are trying to solve, not only the button you would
like. Which core, probe and RTOS you use matters, since most features depend
on what the connected silicon can do.

## Questions

Questions are welcome as issues too. Say what you tried and what you are
trying to learn.

## What happens next

We label each issue by product and confirm bugs on real hardware where we
can. When a fix ships, the issue is closed with the version that contains it.
If we need more detail, we will ask in the thread; issues with no reply for a
long time may be closed and can be reopened at any time.

## Security

For anything you believe is a security problem, do not open a public issue.
Contact BKPT Labs through [bkptlabs.com](https://bkptlabs.com) instead.
