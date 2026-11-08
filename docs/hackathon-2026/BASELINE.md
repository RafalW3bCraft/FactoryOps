# FactoryOps readiness record — November 7, 2026

## Verdict and candidate identity

**Hackathon: approximately 70% ready; submission blocked by the genuine four-agent
workflow, linked-human decision, reviewed video and final submission.**
**Production: approximately 55% ready; release blocked by unverified native
permissions, trusted host deployment and live recovery.** These are judgement
estimates of completed work, not certifications or measured reliability.

The authorized checkout is `/home/victim/factoryops-main`, branch `main`, HEAD
`0a0907fdf72d4950b3351514305da22d5918a134`. The operator externally committed
that revision between work sessions; the assistant issued no Factory commit/push.
Current additional changes remain uncommitted/unpushed. Earlier base:
`197601dcd264044397943c3c7932ceed704a75c2`; event audit base:
`0bf8841ee584669b2786429f7ea677fdd4210de2`.

Current implementation fingerprint: `7bc2993b265b05b5d4df387862457a5ece0531d61055f08928a6d5c5195aff4b`.
The private manifest lists each measured file under
`/home/victim/factoryops-evidence/current-implementation-manifest.json`.
It includes implementation, tests, resources and configuration; operator/history
Markdown is excluded. A commit SHA alone does not identify these working edits.
The frozen installed runtime is `/home/victim/.local/share/factoryops/demo-runtime`.
It contains the wheel and isolated Python environment, not another source clone.
At the operator's later request, old clones/fixtures were archived and removed;
the original shared checkout deletions remain preserved.

## Verified, inferred and unknown

**Verified local:** 234 tests and 13 subtests passed; coverage 88.66%. All ten commands below exited 0 in the repeated final gate. An earlier
formatting failure was corrected before this successful repeat. The full sandbox dependency/image build succeeded after
bounded download retries; actual container containment and two-UID probes ran.
These are local checks, not live native agent or human decisions.

**Verified setup:** Switch Console 0.40.1/core 0.31.0 running; actual local server
`http://localhost:40735/health` returns HTTP 200. Discord is connected and
`@rafal_init` is linked. Template version 4 created Foreman, Smith, Inspector and
Stresser plus private `factoryops-demo-engineering`. All four show Running.
Discord API data confirms @everyone view access denied and two explicitly allowed
members (operator/bot). The real kickoff started Foreman's native session and
requested permission `A1` for `pwd && cat AGENTS.md` in the disposable workspace.

**Inference:** after the operator approves appropriate native tools, the available
seats should execute the supervised inventory workflow. A Running label and
permission request do not prove a completed task or four responding seats.

**Unknown/pending:** four fresh addressed replies, actual handoffs/RED/GREEN/
same-SHA checks, genuine later candidate approval, reviewed video and submission
receipt. Historical buddy direct-chat posting failures are retained as failures.
The official deadline was November 7 at 13:29 EST; it has passed. Late acceptance
requires organizer confirmation; no submission is claimed.

## Mandatory hackathon requirements

PASS means evidence exists; FAIL means currently incomplete; UNKNOWN means the
operator or actual event receipt must supply evidence.

| Requirement | Result | Evidence / remaining action |
|---|---|---|
| Real task by at least one AI agent and a human through Switch/team chat | FAIL | No completed FactoryOps native workflow captured yet |
| Switch central to the submitted workflow | FAIL | Native four-agent template is implemented/imported; actual run pending |
| Track 01 practical business workflow | PARTIAL | Inventory issue scenario implemented; demonstrated business result pending |
| Clear README/reproduction instructions | PASS locally | README and canonical runbook corrected from executed setup; final published revision pending |
| Demonstration video and repository/submission deliverables | FAIL | Recorder works; genuine workflow video/public links/submission receipt pending |
| Team size/eligibility/registration and work during event | UNKNOWN | Operator confirmation and provenance required; existing agents/libraries/templates are allowed, Switch workflow must be event work |
| Deadline | UNKNOWN | Submission receipt must precede November 7, 2026, 13:29 EST |

[Official event requirements](https://www.wemakedevs.org/hackathons/switch).
Track fit is a judging consideration; local test coverage is a project quality
gate, not a substitute for the event's human/AI workflow requirement.

## Current automated commands and exits

Executed in `/home/victim/factoryops-main` with Python 3.12.14 and uv 0.12.10.
Test TMPDIR: `/home/victim/.local/share/factoryops/tests`.

| Actual command | Exit | Result |
|---|---:|---|
| `uv run --frozen ruff check .` | 0 | Passed |
| `uv run --frozen ruff format --check .` | 0 | Passed |
| `uv run --frozen mypy src tests` | 0 | Passed |
| `uv run --frozen shellcheck *.sh scripts/*.sh` | 0 | Actual expanded argv retained in JSON |
| `TMPDIR="$HOME/.local/share/factoryops/tests" uv run --frozen pytest -q --cov=src --cov-fail-under=85` | 0 | 234 passed, 13 subtests; 88.66% |
| `uv run --frozen pip-audit` | 0 | No known dependency vulnerabilities; local Factory package skipped because not on PyPI |
| `uv build` | 0 | Wheel and source distribution built |
| `uv run --frozen python scripts/sync_assets.py --check` | 0 | Canonical/package copies agree |
| `uv run --frozen python scripts/check_supply_chain.py` | 0 | 78 lock/export/SBOM versions agree |
| `git diff --check` | 0 | Passed |

Exact argv, elapsed time and exit codes: `current-final-checks.json`; command
output: `current-final-*.log` in private evidence. Mypy also passed with the new
recorder/principal-probe scripts included (45 files). Bandit 1.9.4 last scan
exited 1: **16 LOW, 0 MEDIUM/HIGH** alerts; this is not a zero-finding pass.
The original installed runtime smoke created a real fixture and matched all 65
package source/resource files at freeze. The active supervised runtime remains
unchanged; `verification.py` and `workflow.py` now differ because new background
hardening is tested in main. A separate disposable installed-wheel environment
passed CLI, finite-timeout rejection and real fixture initialization (all exits
0), without changing that live runtime. No mutable source import was used.
Final container and independent-review results are separate evidence.
No fresh remote CI result is asserted for these uncommitted edits.

## Implementation and remaining proof

| Feature | State | Actual evidence / limit |
|---|---|---|
| Native Foreman/Smith/Inspector/Stresser, sibling addressing, bypass off | Provisioned; workflow pending | Four native seats Running; private room; initial Foreman command awaits permission |
| Supervised/enforced mode consistency | Implemented | Local mode/mismatch tests; supervised report has limited procedural authority |
| Canonical fixture paths, symlink checks, Git relationships, atomic metadata | Implemented | Real disposable Git regression tests; advisory same-UID protection |
| Native `.switch` runtime state | Implemented | Regression preserves ignored runtime files through candidate preparation |
| Independent tooling path in Console | Implemented | RED then GREEN regression; corrected template saved as version 4 |
| Exact-revision, credential-free bounded execution | Implemented locally | Real Podman execution/limits/cleanup; not native provider isolation |
| Durable candidate/attempt-bound ledger and signed report | Implemented; live unverified | Synthetic authenticated event/replay/restart/expiry tests |
| Required-seat freshness and strict diagnostics | Implemented; live unverified | Four opaque identities, challenge freshness, durable retry budget and idle-stream tests |
| Cross-principal read-only candidate access | Partial | Real container UIDs 1000/1001: readonly source succeeds, mutation/private sentinel access denied; host deployment pending |
| Source/image/package/ECC reproducibility | Implemented locally | Frozen builds, resources, non-overwrite tests and supply parity; image identity must match final wheel |
| Legacy Band/OpenCode lifecycle | Implemented legacy path | Owned-process/descendant tests; unsafe host execution remains explicit opt-in |
| Monitoring, backup/restore, real observer recovery, native permissions | Partial/unverified | Production acceptance still required |

Independent development Inspector and Stresser previously returned **LOCAL PASS**
for a bounded core review, each independently running 40 tests and 4 subtests
(exit 0). Their Git-fixture sandbox limits are stated in the reports. These
reviewers are not the native Switch Inspector/Stresser seats. Final independent Inspector/Stresser reviews each passed 45 tests (one
deselected) and verified 139 relevant file hashes before/after, with no new
findings in scope. Fixture initialization was inspected rather than rerun
inside their Git-marked review sandbox; root executed the actual installed test.

## Ordered remaining work

| Priority | Exact files / finding | Acceptance test |
|---|---|---|
| P0 submission | `switch/factoryops.template.yaml`, `docs/hackathon-2026/LIVE_DEMO_EVIDENCE.md`: missing real run | Link genuine human; create four seats/room; four addressed replies within 120 s; real Foreman handoff, Smith RED/GREEN/full SHA; Inspector/Stresser execute independently at same SHA; approval withheld then actual human decides; fresh post-idle response |
| P0 submission | `README.md`, `DEMO_RUNBOOK.md`, live record: video/public delivery pending | Record actual workflow with `scripts/record_demo.py`; review secrets and claims; operator authorizes publication, supplies public links and submission receipt |
| P0 production | `src/factory/switch_gate.py`, `workflow.py`, `verification.py`, `SECURITY.md`: host trust boundary unproved | Trusted controller code/config/state/key under separate OS principal; native tools denied controller/provider secrets and external disposable sentinels; do not rely on prompt rules or permission bits |
| P1 | `switch_gate.py`, `workflow.py`: actual authenticated observer/seat recovery unverified | Real opaque identity/room mapping, stopped-seat failure, idle heartbeat, duplicate/reconnect, restart, changed candidate and takeover; no stale or duplicate authorization |
| P1 | `Dockerfile.sandbox`, `Dockerfile.verifier`, `scripts/verify_containment.py`: exact final deployment proof | Final wheel installed outside source; image package hashes match; immutable-ID containment/limits/cleanup pass; documented operator lifecycle |
| P1 | `workflow.py`, `switch_gate.py`, `DEMO_RUNBOOK.md`: operational recovery | Backup/restore actual state, retained evidence/redacted logs, failure visibility and supported stop/restart; do not promise reboot persistence |
| P2 | `verification.py`, `workflow.py`, operator docs: maintainability/capacity | Review remaining LOW scan alerts, profile representative workloads, state capacity/recovery goals and improve structure without weakening controls |

## Manual interventions

1. Identity is already linked as `@rafal_init`. Approve the genuine initial native
   tool request after review; retain disabled bypass. Existing bot credentials
   stay in Switch, not `.env`.
2. Restrict the dedicated test channel, create the template once, confirm normal
   tool approvals and available existing-account capacity.
3. The operator must personally decide the identified candidate after both
   independent native checks; no assistant-generated human approval.
4. Review the real recording, confirm event/team eligibility, separately authorize
   Factory publication, submit and retain the actual receipt.
5. Production requires separate trusted host ownership and authenticated observer
   setup, effective native containment and recovery evidence.

## Next implementation prompt

> Work only in `/home/victim/factoryops-main` on main; no commits/pushes or changes
> to preserved checkouts/runtime. Read AGENTS.md and ECC TDD/security/verification
> guidance. Start from HEAD0a0907fdf72d4950b3351514305da22d5918a134 plus the current
> fingerprinted working changes. First complete the real supervised Switch/Discord
> four-seat run after the operator reviews native tool permissions; capture actual same-SHA RED/GREEN,
> independent verdicts and later genuine human decision. Fix only reproduced
> blockers test-first; never manufacture messages, approvals or a demo video.
> Then deploy the trusted observer under a separate OS principal, prove native
> tools cannot read controller keys/state/code or provider secrets, exercise real
> recovery/stopped-seat/takeover negatives and final immutable-image containment.
> Run the full documented gate, installed-wheel smoke and independent local
> Inspector/Stresser reviews; update canonical status/runbook/README from actual
> results. Keep publication/submission and human approval pending for the operator.

## Documentation ownership

All 105 Markdown files were inventoried: 43 canonical ECC toolkit files, 4 legacy
mandates, 47 packaged copies and 11 operator/history documents. Active guidance
was corrected; history/upstream skills retained, three real ECC links fixed,
and generated copies synchronized. Examples remain explicitly illustrative.

- `AGENTS.md`: contributor boundaries.
- `README.md`: entry point; `DEMO_RUNBOOK.md`: single setup/manual-test guide.
- `ARCHITECTURE_AUDIT.md` and `SECURITY.md`: code map/trust boundaries.
- This file: current outcomes/blockers; `LIVE_DEMO_EVIDENCE.md`: actual room evidence.
- `CHANGELOG.md`, `docs/AUDIT.md`, `TDD_EVIDENCE.md`: provenance/history.

## Cleanup verification and additional regressions

`cleanup-result.json` records 12 removed directories: three source clones, eight
old inventory fixtures and the old test scratch. Source differences and fixture
history were archived with SHA-256 manifests and reread verification before
removal. `factoryops-main` is the only source checkout; `factoryops-evidence` is
retained data. New scratch/runtime/fixture live under `~/.local/share/factoryops`.

New test-first fixes enforce private Discord/Switch room defaults, use the frozen
installed module for verifier preparation, and make `python -m factory.factoryops`
actually execute the CLI. The first module smoke exposed an exit-0 no-op; the
new help/fixture regressions failed before the entry-point fix. Real installed
initialization now created baseline `c77912a946d9d30d846ee497af165616b434a3c7`.
Offline install attempts lacked cached wheels; bounded online installation
retained frozen hashes and TLS, then the wheel install and actual initialization
exited 0. The installed runtime imports no mutable source checkout or credentials.

## Final local verification after cleanup

The final repeated gate exited 0 for all ten recorded commands: 234 tests,
13 subtests and 88.66% coverage. Bandit exited 1 with 16 LOW and no MEDIUM/HIGH
findings. The original frozen runtime matched all 65 package files at freeze;
its two background-hardening differences are explicitly recorded above. Native Switch
0.31 template lint returned no errors/warnings. Both independent bounded reviews
passed 45 tests each and matched 139 hashes; no live/production clearance.

Actual isolation probes passed on immutable image
`sha256:b0a97104708786cf5d26eeafbf47a5854eeda85db4e054715280e8e7348b1531`:
nonroot, read-only, network/host sentinel denied, no credential environment/socket,
resource limits, timeout/output cap and confirmed cleanup. Final image build
exited 0 using the tested wheel and existing pinned base dependencies offline.
These probes do not establish native-provider permissions or host principal
separation. The temporary localhost-only form automation endpoint was closed;
Console was relaunched normally with the requested secret-store option.

Evidence: `current-final-checks.json`, `current-final-coverage.log`,
`continue-bandit.json`, `continue-frozen-runtime-parity.json`,
`cleanup-final-image-build.json`, `cleanup-final-containment.json`,
`cleanup-independent-reviews/`, `cleanup-markdown-audit.json` and
`console-automation-session.json` under the private evidence directory.

## Latest recovery repair and validation

An independent local restore probe reproduced a P1 authorization gap: a restored
approval could become readable after `connection_ready()` refreshed health and
before the gate cleared old readiness. A new real-SQLite/signed-artifact test
failed at that exact independent read (exit 1). The repair atomically clears old
request, approval and readiness in the transaction that restores health, retaining
receipts/verdicts and historical evidence. The regression passes; reconnect now
requires fresh readiness and a new human decision. Source: `workflow.py`; tests:
`test_required_seats.py`, `test_workflow.py`. These use synthetic platform events,
not real human decisions.

Separately, NaN/infinite timeouts previously executed commands without a finite
deadline. The new parameterized regression initially returned 2 failures and
3 passes (exit 1); finite validation now rejects them before process creation.
The targeted verifier suite passed 14 tests (exit 0). An intermediate restore
test had an incorrect assumption about nullable history entries; that test was
corrected before the successful full gate.

The latest full gate passed 234 tests and 13 subtests with 88.66% coverage; all ten
commands exited 0. Independent Inspector reran 54 targeted tests and the original
restore race; Stresser reran 43 tests and extra timeout/replay/restore probes;
both gave bounded LOCAL PASS, exit 0. These development reviewers are separate
from native Switch reviewers. Evidence: `reconnect-final-reviews/`,
`current-final-checks.json`, `continue-wheel-smoke.json`. Bandit 1.9.4 returned
exit 1, still 16 LOW findings and none MEDIUM/HIGH.

The updated wheel's offline image overlay first failed (exit 1) because the base
project virtualenv has no pip. Rebuilding with its existing pinned uv succeeded
(exit 0), without downloads or TLS changes. Current image:
`sha256:13d9bb3e76625b49e6ff407e0c6a0874dbe945aed5988cc47c289d084f45e7e8`.
See `continue-image-build.json` and the retained attempt-1 log. This candidate
has not replaced the frozen live demonstration runtime.

Actual containment on that updated immutable image exited 0: nonroot/read-only,
no credential environment/socket, network and host sentinel denial, memory/PID
limits, timeout/output limits (expected 124), and cleanup exits 0. A separate
in-container package-hash probe matched all 65 current source/resource files,
exit 0. Evidence: `continue-containment-command.json`,
`continue-containment.json`, `continue-image-package-parity.json`. This is
container execution, not native provider clearance. The 105-file Markdown link
recheck found no broken active local links (`continue-markdown-audit.json`).
