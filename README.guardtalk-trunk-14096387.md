GuardTalkOS: symlink trunk-14096387 -> grapheneos.

trunk_staging sets RELEASE_KERNEL_DIR to .../trunk-14096387; the pinned
kernel prebuilt in this tree is .../grapheneos. Same pattern as caiman
(caimito-kernels/6.1/trunk-14096387) and comet.
Reversible: rm the symlink.

NOTE (2026-10-18): this symlink is INVISIBLE to `repo sync` — a sync of this
project deletes the work tree (including this symlink) and re-creates it from
the remote. Re-apply after any sync of device/google/tangorpro-kernels.
