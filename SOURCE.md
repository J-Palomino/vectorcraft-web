Web build of VectorCraft v0.17.0 (https://github.com/storytold/vectorcraft/releases/tag/v0.17.0)
with one change: new documents save as Illustrator `.ai` (PDF-compatible) by default instead of
`.vectorcraft`. The change is `patches/ai-default-save.patch` (browser builds only; desktop unchanged).

Built with Rust 1.95.0, trunk 0.21.14 and craft-fonts a71c20e30af613287c504f7e685ca8fad77752bc,
as the upstream release workflow does:

    git apply patches/ai-default-save.patch      # in a v0.17.0 checkout
    CRAFT_FONTS_DIR=<craft-fonts checkout> CRAFT_FONTS_REQUIRED=1 packaging/web/package.sh

VectorCraft is dual-licensed MIT / Apache-2.0 (see LICENSE-MIT, LICENSE-APACHE, NOTICE).
