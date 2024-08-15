# Supernote A5X 2024 Planner for a lefty

I use nixos anyway on my environments, so my approach to building the PDFs was

`nix develop` to get the development environment to build from the `flake.nix` derivation. Then from the shell it enters you into, run the following command.

I don't remember the different files I played with to make it lefthanded. You can probably do a diff against the original source. https://github.com/kudrykv/latex-yearly-planner

```bash

# This created a good working A5X planner for a lefty.
# It would be nice if the mos_02_quarterly.tpl was adjusted to show the calendars on the right.
[stuart@T14 latex-yearly-planner]$ PLANNER_YEAR="2024" PASSES="1" CFG="cfg/base.yaml,cfg/rm2_ddvk_lh.base.yaml,cfg/template_months_on_side.yaml,cfg/sn_a5x.mos.default.dailycal.yaml" NAME="test_sn5_ddvk_lh.mos.default.dailycal.2024" ./single.sh

```

## Credit

All credit goes to the author - all I have done it adjusted some of the files to make a lefthanded version of the generated daily planner. [The original project is here](https://github.com/kudrykv)

Thanks  Vitaliy Kudryk!

Cheers,
Stuart
