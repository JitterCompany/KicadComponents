# attestations/

Signed pin tables for parts used with this library, written by `bomcheck` (in
[pcb_release](https://github.com/JitterCompany/pcb_release), `scripts/bomcheck/`).

    reference/datasheet/<MPN>.toml   what the datasheet says about one MPN: pin
                                     names, polarity mark, internal connections,
                                     who checked it and against which document

A table does not depend on a board. A board that uses this library as a
submodule reads these tables, so a part checked once is checked for every
board. A board can still keep its own table for an MPN; that one wins.

New tables arrive from the bomcheck wizard on a board: it saves tables for
library parts here, in the submodule. Commit them on a branch and open a PR.
The board picks them up after its submodule is updated.

Format: `scripts/bomcheck/FORMAT.md` in pcb_release.
