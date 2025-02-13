# Table of Contents

<!-- toc -->

- [LSP](#lsp)
  * [LSP Installer](#lsp-installer)
  * [LSP Feature Extension UI](#lsp-feature-extension-ui)
    + [Diagnostics](#diagnostics)
    + [Definition, Reference](#definition-reference)
    + [Code action](#code-action)
    + [Hint](#hint)
    + [Hover Doc](#hover-doc)
    + [Formatting](#formatting)
    + [Rename](#rename)
    + [textDocument](#textdocument)
      - [LinkedEditingRange](#linkededitingrange)
    + [window](#window)
      - [logMessage](#logmessage)
    + [Semantic Token](#semantic-token)
  * [LSP Progress](#lsp-progress)
  * [LSP Log](#lsp-log)
  * [Local LSP Config](#local-lsp-config)
- [Command](#command)
  * [Disable/Enable](#disableenable)
- [Pre-configuration](#pre-configuration)
- [Backwards Compatibility](#backwards-compatibility)

<!-- tocstop -->

## LSP

- [neovim/nvim-lspconfig](https://github.com/neovim/nvim-lspconfig) ![](https://img.shields.io/github/stars/neovim/nvim-lspconfig) ![](https://img.shields.io/github/last-commit/neovim/nvim-lspconfig) ![](https://img.shields.io/github/commit-activity/y/neovim/nvim-lspconfig)

### LSP Installer

- [williamboman/mason.nvim(lsp installer)](https://github.com/williamboman/mason.nvim) ![](https://img.shields.io/github/stars/williamboman/mason.nvim) ![](https://img.shields.io/github/last-commit/williamboman/mason.nvim) ![](https://img.shields.io/github/commit-activity/y/williamboman/mason.nvim)
  - [williamboman/mason-lspconfig.nvim](https://github.com/williamboman/mason-lspconfig.nvim) ![](https://img.shields.io/github/stars/williamboman/mason-lspconfig.nvim) ![](https://img.shields.io/github/last-commit/williamboman/mason-lspconfig.nvim) ![](https://img.shields.io/github/commit-activity/y/williamboman/mason-lspconfig.nvim)
- [lspcontainers/lspcontainers.nvim](https://github.com/lspcontainers/lspcontainers.nvim) ![](https://img.shields.io/github/stars/lspcontainers/lspcontainers.nvim) ![](https://img.shields.io/github/last-commit/lspcontainers/lspcontainers.nvim) ![](https://img.shields.io/github/commit-activity/y/lspcontainers/lspcontainers.nvim)
- [dundalek/lazy-lsp.nvim](https://github.com/dundalek/lazy-lsp.nvim) ![](https://img.shields.io/github/stars/dundalek/lazy-lsp.nvim) ![](https://img.shields.io/github/last-commit/dundalek/lazy-lsp.nvim) ![](https://img.shields.io/github/commit-activity/y/dundalek/lazy-lsp.nvim)

### LSP Feature Extension UI

- [nvimdev/lspsaga.nvim](https://github.com/nvimdev/lspsaga.nvim) ![](https://img.shields.io/github/stars/nvimdev/lspsaga.nvim) ![](https://img.shields.io/github/last-commit/nvimdev/lspsaga.nvim) ![](https://img.shields.io/github/commit-activity/y/nvimdev/lspsaga.nvim)
- [kkharji/lspsaga.nvim](https://github.com/kkharji/lspsaga.nvim) ![](https://img.shields.io/github/stars/kkharji/lspsaga.nvim) ![](https://img.shields.io/github/last-commit/kkharji/lspsaga.nvim) ![](https://img.shields.io/github/commit-activity/y/kkharji/lspsaga.nvim)
- [folke/trouble.nvim](https://github.com/folke/trouble.nvim) ![](https://img.shields.io/github/stars/folke/trouble.nvim) ![](https://img.shields.io/github/last-commit/folke/trouble.nvim) ![](https://img.shields.io/github/commit-activity/y/folke/trouble.nvim)
  - [EthanJWright/toolwindow.nvim](https://github.com/EthanJWright/toolwindow.nvim) ![](https://img.shields.io/github/stars/EthanJWright/toolwindow.nvim) ![](https://img.shields.io/github/last-commit/EthanJWright/toolwindow.nvim) ![](https://img.shields.io/github/commit-activity/y/EthanJWright/toolwindow.nvim)
- [DNLHC/glance.nvim](https://github.com/DNLHC/glance.nvim) ![](https://img.shields.io/github/stars/DNLHC/glance.nvim) ![](https://img.shields.io/github/last-commit/DNLHC/glance.nvim) ![](https://img.shields.io/github/commit-activity/y/DNLHC/glance.nvim)
- [ray-x/navigator.lua](https://github.com/ray-x/navigator.lua) ![](https://img.shields.io/github/stars/ray-x/navigator.lua) ![](https://img.shields.io/github/last-commit/ray-x/navigator.lua) ![](https://img.shields.io/github/commit-activity/y/ray-x/navigator.lua)
- [williamboman/warden.nvim](https://github.com/williamboman/warden.nvim) ![](https://img.shields.io/github/stars/williamboman/warden.nvim) ![](https://img.shields.io/github/last-commit/williamboman/warden.nvim) ![](https://img.shields.io/github/commit-activity/y/williamboman/warden.nvim)
- [gfanto/fzf-lsp.nvim](https://github.com/gfanto/fzf-lsp.nvim) ![](https://img.shields.io/github/stars/gfanto/fzf-lsp.nvim) ![](https://img.shields.io/github/last-commit/gfanto/fzf-lsp.nvim) ![](https://img.shields.io/github/commit-activity/y/gfanto/fzf-lsp.nvim)
- [RishabhRD/nvim-lsputils](https://github.com/RishabhRD/nvim-lsputils) ![](https://img.shields.io/github/stars/RishabhRD/nvim-lsputils) ![](https://img.shields.io/github/last-commit/RishabhRD/nvim-lsputils) ![](https://img.shields.io/github/commit-activity/y/RishabhRD/nvim-lsputils)
- [seblj/nvim-lsp-extras](https://github.com/seblj/nvim-lsp-extras) ![](https://img.shields.io/github/stars/seblj/nvim-lsp-extras) ![](https://img.shields.io/github/last-commit/seblj/nvim-lsp-extras) ![](https://img.shields.io/github/commit-activity/y/seblj/nvim-lsp-extras)
- [jinzhongjia/LspUI.nvim](https://github.com/jinzhongjia/LspUI.nvim) ![](https://img.shields.io/github/stars/jinzhongjia/LspUI.nvim) ![](https://img.shields.io/github/last-commit/jinzhongjia/LspUI.nvim) ![](https://img.shields.io/github/commit-activity/y/jinzhongjia/LspUI.nvim)
- [nvim-jo/lspsystem.nvim](https://github.com/nvim-jo/lspsystem.nvim) ![](https://img.shields.io/github/stars/nvim-jo/lspsystem.nvim) ![](https://img.shields.io/github/last-commit/nvim-jo/lspsystem.nvim) ![](https://img.shields.io/github/commit-activity/y/nvim-jo/lspsystem.nvim)

#### Diagnostics

- [jose-elias-alvarez/null-ls.nvim(Diagnostics)](https://github.com/jose-elias-alvarez/null-ls.nvim) ![](https://img.shields.io/github/stars/jose-elias-alvarez/null-ls.nvim) ![](https://img.shields.io/github/last-commit/jose-elias-alvarez/null-ls.nvim) ![](https://img.shields.io/github/commit-activity/y/jose-elias-alvarez/null-ls.nvim)
- [onsails/diaglist.nvim](https://github.com/onsails/diaglist.nvim) ![](https://img.shields.io/github/stars/onsails/diaglist.nvim) ![](https://img.shields.io/github/last-commit/onsails/diaglist.nvim) ![](https://img.shields.io/github/commit-activity/y/onsails/diaglist.nvim)
- [lithammer/nvim-diagnosticls](https://github.com/lithammer/nvim-diagnosticls) ![](https://img.shields.io/github/stars/lithammer/nvim-diagnosticls) ![](https://img.shields.io/github/last-commit/lithammer/nvim-diagnosticls) ![](https://img.shields.io/github/commit-activity/y/lithammer/nvim-diagnosticls)
- [kaputi/e-kaput.nvim](https://github.com/kaputi/e-kaput.nvim) ![](https://img.shields.io/github/stars/kaputi/e-kaput.nvim) ![](https://img.shields.io/github/last-commit/kaputi/e-kaput.nvim) ![](https://img.shields.io/github/commit-activity/y/kaputi/e-kaput.nvim)
- [Mofiqul/trld.nvim](https://github.com/Mofiqul/trld.nvim) ![](https://img.shields.io/github/stars/Mofiqul/trld.nvim) ![](https://img.shields.io/github/last-commit/Mofiqul/trld.nvim) ![](https://img.shields.io/github/commit-activity/y/Mofiqul/trld.nvim)
- [Maan2003/lsp_lines.nvim](https://github.com/Maan2003/lsp_lines.nvim) ![](https://img.shields.io/github/stars/Maan2003/lsp_lines.nvim) ![](https://img.shields.io/github/last-commit/Maan2003/lsp_lines.nvim) ![](https://img.shields.io/github/commit-activity/y/Maan2003/lsp_lines.nvim)
- [ksyasuda/lsp_lines.nvim](https://github.com/ksyasuda/lsp_lines.nvim) ![](https://img.shields.io/github/stars/ksyasuda/lsp_lines.nvim) ![](https://img.shields.io/github/last-commit/ksyasuda/lsp_lines.nvim) ![](https://img.shields.io/github/commit-activity/y/ksyasuda/lsp_lines.nvim)
- [Kasama/nvim-custom-diagnostic-highlight](https://github.com/Kasama/nvim-custom-diagnostic-highlight) ![](https://img.shields.io/github/stars/Kasama/nvim-custom-diagnostic-highlight) ![](https://img.shields.io/github/last-commit/Kasama/nvim-custom-diagnostic-highlight) ![](https://img.shields.io/github/commit-activity/y/Kasama/nvim-custom-diagnostic-highlight)
- [cseickel/diagnostic-window.nvim](https://github.com/cseickel/diagnostic-window.nvim) ![](https://img.shields.io/github/stars/cseickel/diagnostic-window.nvim) ![](https://img.shields.io/github/last-commit/cseickel/diagnostic-window.nvim) ![](https://img.shields.io/github/commit-activity/y/cseickel/diagnostic-window.nvim)
- [zbirenbaum/neodim](https://github.com/zbirenbaum/neodim) ![](https://img.shields.io/github/stars/zbirenbaum/neodim) ![](https://img.shields.io/github/last-commit/zbirenbaum/neodim) ![](https://img.shields.io/github/commit-activity/y/zbirenbaum/neodim)
- [WhoIsSethDaniel/toggle-lsp-diagnostics.nvim](https://github.com/WhoIsSethDaniel/toggle-lsp-diagnostics.nvim) ![](https://img.shields.io/github/stars/WhoIsSethDaniel/toggle-lsp-diagnostics.nvim) ![](https://img.shields.io/github/last-commit/WhoIsSethDaniel/toggle-lsp-diagnostics.nvim) ![](https://img.shields.io/github/commit-activity/y/WhoIsSethDaniel/toggle-lsp-diagnostics.nvim)
- [casonadams/simple-diagnostics.nvim](https://github.com/casonadams/simple-diagnostics.nvim) ![](https://img.shields.io/github/stars/casonadams/simple-diagnostics.nvim) ![](https://img.shields.io/github/last-commit/casonadams/simple-diagnostics.nvim) ![](https://img.shields.io/github/commit-activity/y/casonadams/simple-diagnostics.nvim)
- [stefanwatt/lsp-lines.nvim](https://github.com/stefanwatt/lsp-lines.nvim) ![](https://img.shields.io/github/stars/stefanwatt/lsp-lines.nvim) ![](https://img.shields.io/github/last-commit/stefanwatt/lsp-lines.nvim) ![](https://img.shields.io/github/commit-activity/y/stefanwatt/lsp-lines.nvim)
- [nicolomaioli/wtfm.nvim](https://github.com/nicolomaioli/wtfm.nvim) ![](https://img.shields.io/github/stars/nicolomaioli/wtfm.nvim) ![](https://img.shields.io/github/last-commit/nicolomaioli/wtfm.nvim) ![](https://img.shields.io/github/commit-activity/y/nicolomaioli/wtfm.nvim)
- [TomDeneire/notify-diagnostics.nvim](https://github.com/TomDeneire/notify-diagnostics.nvim) ![](https://img.shields.io/github/stars/TomDeneire/notify-diagnostics.nvim) ![](https://img.shields.io/github/last-commit/TomDeneire/notify-diagnostics.nvim) ![](https://img.shields.io/github/commit-activity/y/TomDeneire/notify-diagnostics.nvim)
- [chikko80/error-lens.nvim](https://github.com/chikko80/error-lens.nvim) ![](https://img.shields.io/github/stars/chikko80/error-lens.nvim) ![](https://img.shields.io/github/last-commit/chikko80/error-lens.nvim) ![](https://img.shields.io/github/commit-activity/y/chikko80/error-lens.nvim)
- [isaksamsten/better-virtual-text.nvim](https://github.com/isaksamsten/better-virtual-text.nvim) ![](https://img.shields.io/github/stars/isaksamsten/better-virtual-text.nvim) ![](https://img.shields.io/github/last-commit/isaksamsten/better-virtual-text.nvim) ![](https://img.shields.io/github/commit-activity/y/isaksamsten/better-virtual-text.nvim)
- [luozhiya/lsp-virtual-improved.nvim](https://github.com/luozhiya/lsp-virtual-improved.nvim) ![](https://img.shields.io/github/stars/luozhiya/lsp-virtual-improved.nvim) ![](https://img.shields.io/github/last-commit/luozhiya/lsp-virtual-improved.nvim) ![](https://img.shields.io/github/commit-activity/y/luozhiya/lsp-virtual-improved.nvim)
- [yorickpeterse/nvim-dd](https://github.com/yorickpeterse/nvim-dd) ![](https://img.shields.io/github/stars/yorickpeterse/nvim-dd) ![](https://img.shields.io/github/last-commit/yorickpeterse/nvim-dd) ![](https://img.shields.io/github/commit-activity/y/yorickpeterse/nvim-dd)

#### Definition, Reference

- [rmagatti/goto-preview](https://github.com/rmagatti/goto-preview) ![](https://img.shields.io/github/stars/rmagatti/goto-preview) ![](https://img.shields.io/github/last-commit/rmagatti/goto-preview) ![](https://img.shields.io/github/commit-activity/y/rmagatti/goto-preview)
- [ojroques/nvim-lspfuzzy](https://github.com/ojroques/nvim-lspfuzzy) ![](https://img.shields.io/github/stars/ojroques/nvim-lspfuzzy) ![](https://img.shields.io/github/last-commit/ojroques/nvim-lspfuzzy) ![](https://img.shields.io/github/commit-activity/y/ojroques/nvim-lspfuzzy)
- [wiliamks/nice-reference.nvim](https://github.com/wiliamks/nice-reference.nvim) ![](https://img.shields.io/github/stars/wiliamks/nice-reference.nvim) ![](https://img.shields.io/github/last-commit/wiliamks/nice-reference.nvim) ![](https://img.shields.io/github/commit-activity/y/wiliamks/nice-reference.nvim)
- [gbrlsnchs/telescope-lsp-handlers.nvim](https://github.com/gbrlsnchs/telescope-lsp-handlers.nvim) ![](https://img.shields.io/github/stars/gbrlsnchs/telescope-lsp-handlers.nvim) ![](https://img.shields.io/github/last-commit/gbrlsnchs/telescope-lsp-handlers.nvim) ![](https://img.shields.io/github/commit-activity/y/gbrlsnchs/telescope-lsp-handlers.nvim)
- [edolphin-ydf/goimpl.nvim](https://github.com/edolphin-ydf/goimpl.nvim) ![](https://img.shields.io/github/stars/edolphin-ydf/goimpl.nvim) ![](https://img.shields.io/github/last-commit/edolphin-ydf/goimpl.nvim) ![](https://img.shields.io/github/commit-activity/y/edolphin-ydf/goimpl.nvim)
- [hrsh7th/nvim-gtd](https://github.com/hrsh7th/nvim-gtd) ![](https://img.shields.io/github/stars/hrsh7th/nvim-gtd) ![](https://img.shields.io/github/last-commit/hrsh7th/nvim-gtd) ![](https://img.shields.io/github/commit-activity/y/hrsh7th/nvim-gtd)
- [Davidyz/lsp-location-handler.nvim](https://github.com/Davidyz/lsp-location-handler.nvim) ![](https://img.shields.io/github/stars/Davidyz/lsp-location-handler.nvim) ![](https://img.shields.io/github/last-commit/Davidyz/lsp-location-handler.nvim) ![](https://img.shields.io/github/commit-activity/y/Davidyz/lsp-location-handler.nvim)
- [VidocqH/lsp-lens.nvim](https://github.com/VidocqH/lsp-lens.nvim) ![](https://img.shields.io/github/stars/VidocqH/lsp-lens.nvim) ![](https://img.shields.io/github/last-commit/VidocqH/lsp-lens.nvim) ![](https://img.shields.io/github/commit-activity/y/VidocqH/lsp-lens.nvim)
- [KostkaBrukowa/definition-or-references.nvim](https://github.com/KostkaBrukowa/definition-or-references.nvim) ![](https://img.shields.io/github/stars/KostkaBrukowa/definition-or-references.nvim) ![](https://img.shields.io/github/last-commit/KostkaBrukowa/definition-or-references.nvim) ![](https://img.shields.io/github/commit-activity/y/KostkaBrukowa/definition-or-references.nvim)

#### Code action

- [jose-elias-alvarez/null-ls.nvim(Code actions)](https://github.com/jose-elias-alvarez/null-ls.nvim) ![](https://img.shields.io/github/stars/jose-elias-alvarez/null-ls.nvim) ![](https://img.shields.io/github/last-commit/jose-elias-alvarez/null-ls.nvim) ![](https://img.shields.io/github/commit-activity/y/jose-elias-alvarez/null-ls.nvim)
- [kosayoda/nvim-lightbulb](https://github.com/kosayoda/nvim-lightbulb) ![](https://img.shields.io/github/stars/kosayoda/nvim-lightbulb) ![](https://img.shields.io/github/last-commit/kosayoda/nvim-lightbulb) ![](https://img.shields.io/github/commit-activity/y/kosayoda/nvim-lightbulb)
- [weilbith/nvim-code-action-menu](https://github.com/weilbith/nvim-code-action-menu) ![](https://img.shields.io/github/stars/weilbith/nvim-code-action-menu) ![](https://img.shields.io/github/last-commit/weilbith/nvim-code-action-menu) ![](https://img.shields.io/github/commit-activity/y/weilbith/nvim-code-action-menu)
- [RishabhRD/lspactions](https://github.com/RishabhRD/lspactions) ![](https://img.shields.io/github/stars/RishabhRD/lspactions) ![](https://img.shields.io/github/last-commit/RishabhRD/lspactions) ![](https://img.shields.io/github/commit-activity/y/RishabhRD/lspactions)
- [nyarthan/telescope-code-actions.nvim](https://github.com/nyarthan/telescope-code-actions.nvim) ![](https://img.shields.io/github/stars/nyarthan/telescope-code-actions.nvim) ![](https://img.shields.io/github/last-commit/nyarthan/telescope-code-actions.nvim) ![](https://img.shields.io/github/commit-activity/y/nyarthan/telescope-code-actions.nvim)
- [aznhe21/actions-preview.nvim](https://github.com/aznhe21/actions-preview.nvim) ![](https://img.shields.io/github/stars/aznhe21/actions-preview.nvim) ![](https://img.shields.io/github/last-commit/aznhe21/actions-preview.nvim) ![](https://img.shields.io/github/commit-activity/y/aznhe21/actions-preview.nvim)

#### Hint

- [jubnzv/virtual-types.nvim](https://github.com/jubnzv/virtual-types.nvim) ![](https://img.shields.io/github/stars/jubnzv/virtual-types.nvim) ![](https://img.shields.io/github/last-commit/jubnzv/virtual-types.nvim) ![](https://img.shields.io/github/commit-activity/y/jubnzv/virtual-types.nvim)
- [lvimuser/lsp-inlayhints.nvim](https://github.com/lvimuser/lsp-inlayhints.nvim) ![](https://img.shields.io/github/stars/lvimuser/lsp-inlayhints.nvim) ![](https://img.shields.io/github/last-commit/lvimuser/lsp-inlayhints.nvim) ![](https://img.shields.io/github/commit-activity/y/lvimuser/lsp-inlayhints.nvim)
- [simrat39/inlay-hints.nvim](https://github.com/simrat39/inlay-hints.nvim) ![](https://img.shields.io/github/stars/simrat39/inlay-hints.nvim) ![](https://img.shields.io/github/last-commit/simrat39/inlay-hints.nvim) ![](https://img.shields.io/github/commit-activity/y/simrat39/inlay-hints.nvim)
- [Daniel-Esteban/nvim-inlay-hints](https://github.com/Daniel-Esteban/nvim-inlay-hints) ![](https://img.shields.io/github/stars/Daniel-Esteban/nvim-inlay-hints) ![](https://img.shields.io/github/last-commit/Daniel-Esteban/nvim-inlay-hints) ![](https://img.shields.io/github/commit-activity/y/Daniel-Esteban/nvim-inlay-hints)
- [phenax/nvim-extra-codelens](https://github.com/phenax/nvim-extra-codelens) ![](https://img.shields.io/github/stars/phenax/nvim-extra-codelens) ![](https://img.shields.io/github/last-commit/phenax/nvim-extra-codelens) ![](https://img.shields.io/github/commit-activity/y/phenax/nvim-extra-codelens)
- [27justin/virtuality.nvim](https://github.com/27justin/virtuality.nvim) ![](https://img.shields.io/github/stars/27justin/virtuality.nvim) ![](https://img.shields.io/github/last-commit/27justin/virtuality.nvim) ![](https://img.shields.io/github/commit-activity/y/27justin/virtuality.nvim)

#### Hover Doc

- [jose-elias-alvarez/null-ls.nvim(Hover)](https://github.com/jose-elias-alvarez/null-ls.nvim) ![](https://img.shields.io/github/stars/jose-elias-alvarez/null-ls.nvim) ![](https://img.shields.io/github/last-commit/jose-elias-alvarez/null-ls.nvim) ![](https://img.shields.io/github/commit-activity/y/jose-elias-alvarez/null-ls.nvim)
- [tamago324/lsp-preview-hover-doc.nvim](https://github.com/tamago324/lsp-preview-hover-doc.nvim) ![](https://img.shields.io/github/stars/tamago324/lsp-preview-hover-doc.nvim) ![](https://img.shields.io/github/last-commit/tamago324/lsp-preview-hover-doc.nvim) ![](https://img.shields.io/github/commit-activity/y/tamago324/lsp-preview-hover-doc.nvim)
- [amrbashir/nvim-docs-view](https://github.com/amrbashir/nvim-docs-view) ![](https://img.shields.io/github/stars/amrbashir/nvim-docs-view) ![](https://img.shields.io/github/last-commit/amrbashir/nvim-docs-view) ![](https://img.shields.io/github/commit-activity/y/amrbashir/nvim-docs-view)
- [xiyaowong/link-visitor.nvim](https://github.com/xiyaowong/link-visitor.nvim) ![](https://img.shields.io/github/stars/xiyaowong/link-visitor.nvim) ![](https://img.shields.io/github/last-commit/xiyaowong/link-visitor.nvim) ![](https://img.shields.io/github/commit-activity/y/xiyaowong/link-visitor.nvim)

#### Formatting

- [yioneko/nvim-type-fmt](https://github.com/yioneko/nvim-type-fmt) ![](https://img.shields.io/github/stars/yioneko/nvim-type-fmt) ![](https://img.shields.io/github/last-commit/yioneko/nvim-type-fmt) ![](https://img.shields.io/github/commit-activity/y/yioneko/nvim-type-fmt)
- [aznhe21/lsp-query-format.nvim](https://github.com/aznhe21/lsp-query-format.nvim) ![](https://img.shields.io/github/stars/aznhe21/lsp-query-format.nvim) ![](https://img.shields.io/github/last-commit/aznhe21/lsp-query-format.nvim) ![](https://img.shields.io/github/commit-activity/y/aznhe21/lsp-query-format.nvim)

#### Rename

- [smjonas/inc-rename.nvim](https://github.com/smjonas/inc-rename.nvim) ![](https://img.shields.io/github/stars/smjonas/inc-rename.nvim) ![](https://img.shields.io/github/last-commit/smjonas/inc-rename.nvim) ![](https://img.shields.io/github/commit-activity/y/smjonas/inc-rename.nvim)

#### textDocument

##### LinkedEditingRange

- [hrsh7th/nvim-linkedit](https://github.com/hrsh7th/nvim-linkedit) ![](https://img.shields.io/github/stars/hrsh7th/nvim-linkedit) ![](https://img.shields.io/github/last-commit/hrsh7th/nvim-linkedit) ![](https://img.shields.io/github/commit-activity/y/hrsh7th/nvim-linkedit)

#### window

##### logMessage

- [mhanberg/control-panel.nvim](https://github.com/mhanberg/control-panel.nvim) ![](https://img.shields.io/github/stars/mhanberg/control-panel.nvim) ![](https://img.shields.io/github/last-commit/mhanberg/control-panel.nvim) ![](https://img.shields.io/github/commit-activity/y/mhanberg/control-panel.nvim)

#### Semantic Token

### LSP Progress

- [j-hui/fidget.nvim](https://github.com/j-hui/fidget.nvim) ![](https://img.shields.io/github/stars/j-hui/fidget.nvim) ![](https://img.shields.io/github/last-commit/j-hui/fidget.nvim) ![](https://img.shields.io/github/commit-activity/y/j-hui/fidget.nvim)
- [nvim-lua/lsp-status.nvim](https://github.com/nvim-lua/lsp-status.nvim) ![](https://img.shields.io/github/stars/nvim-lua/lsp-status.nvim) ![](https://img.shields.io/github/last-commit/nvim-lua/lsp-status.nvim) ![](https://img.shields.io/github/commit-activity/y/nvim-lua/lsp-status.nvim)
- [arkav/lualine-lsp-progress](https://github.com/arkav/lualine-lsp-progress) ![](https://img.shields.io/github/stars/arkav/lualine-lsp-progress) ![](https://img.shields.io/github/last-commit/arkav/lualine-lsp-progress) ![](https://img.shields.io/github/commit-activity/y/arkav/lualine-lsp-progress)
- [folke/noice.nvim(mini)](https://github.com/folke/noice.nvim) ![](https://img.shields.io/github/stars/folke/noice.nvim) ![](https://img.shields.io/github/last-commit/folke/noice.nvim) ![](https://img.shields.io/github/commit-activity/y/folke/noice.nvim)
- [mrded/nvim-lsp-notify](https://github.com/mrded/nvim-lsp-notify) ![](https://img.shields.io/github/stars/mrded/nvim-lsp-notify) ![](https://img.shields.io/github/last-commit/mrded/nvim-lsp-notify) ![](https://img.shields.io/github/commit-activity/y/mrded/nvim-lsp-notify)
- [linrongbin16/lsp-progress.nvim](https://github.com/linrongbin16/lsp-progress.nvim) ![](https://img.shields.io/github/stars/linrongbin16/lsp-progress.nvim) ![](https://img.shields.io/github/last-commit/linrongbin16/lsp-progress.nvim) ![](https://img.shields.io/github/commit-activity/y/linrongbin16/lsp-progress.nvim)
- [davidosomething/everandever.nvim](https://github.com/davidosomething/everandever.nvim) ![](https://img.shields.io/github/stars/davidosomething/everandever.nvim) ![](https://img.shields.io/github/last-commit/davidosomething/everandever.nvim) ![](https://img.shields.io/github/commit-activity/y/davidosomething/everandever.nvim)

### LSP Log

- [mhanberg/output-panel.nvim](https://github.com/mhanberg/output-panel.nvim) ![](https://img.shields.io/github/stars/mhanberg/output-panel.nvim) ![](https://img.shields.io/github/last-commit/mhanberg/output-panel.nvim) ![](https://img.shields.io/github/commit-activity/y/mhanberg/output-panel.nvim)

### Local LSP Config

- [folke/neoconf.nvim](https://github.com/folke/neoconf.nvim) ![](https://img.shields.io/github/stars/folke/neoconf.nvim) ![](https://img.shields.io/github/last-commit/folke/neoconf.nvim) ![](https://img.shields.io/github/commit-activity/y/folke/neoconf.nvim)
- [tamago324/nlsp-settings.nvim](https://github.com/tamago324/nlsp-settings.nvim) ![](https://img.shields.io/github/stars/tamago324/nlsp-settings.nvim) ![](https://img.shields.io/github/last-commit/tamago324/nlsp-settings.nvim) ![](https://img.shields.io/github/commit-activity/y/tamago324/nlsp-settings.nvim)

## Command

- [ii14/lsp-command](https://github.com/ii14/lsp-command) ![](https://img.shields.io/github/stars/ii14/lsp-command) ![](https://img.shields.io/github/last-commit/ii14/lsp-command) ![](https://img.shields.io/github/commit-activity/y/ii14/lsp-command)

### Disable/Enable

- [adoyle-h/lsp-toggle.nvim](https://github.com/adoyle-h/lsp-toggle.nvim) ![](https://img.shields.io/github/stars/adoyle-h/lsp-toggle.nvim) ![](https://img.shields.io/github/last-commit/adoyle-h/lsp-toggle.nvim) ![](https://img.shields.io/github/commit-activity/y/adoyle-h/lsp-toggle.nvim)

## Pre-configuration

- [junnplus/nvim-lsp-setup](https://github.com/junnplus/nvim-lsp-setup) ![](https://img.shields.io/github/stars/junnplus/nvim-lsp-setup) ![](https://img.shields.io/github/last-commit/junnplus/nvim-lsp-setup) ![](https://img.shields.io/github/commit-activity/y/junnplus/nvim-lsp-setup)
- [VonHeikemen/lsp-zero.nvim](https://github.com/VonHeikemen/lsp-zero.nvim) ![](https://img.shields.io/github/stars/VonHeikemen/lsp-zero.nvim) ![](https://img.shields.io/github/last-commit/VonHeikemen/lsp-zero.nvim) ![](https://img.shields.io/github/commit-activity/y/VonHeikemen/lsp-zero.nvim)
- [phaazon/poesie.nvim](https://github.com/phaazon/poesie.nvim) ![](https://img.shields.io/github/stars/phaazon/poesie.nvim) ![](https://img.shields.io/github/last-commit/phaazon/poesie.nvim) ![](https://img.shields.io/github/commit-activity/y/phaazon/poesie.nvim)
- [nvim-lua/kickstart.nvim](https://github.com/nvim-lua/kickstart.nvim) ![](https://img.shields.io/github/stars/nvim-lua/kickstart.nvim) ![](https://img.shields.io/github/last-commit/nvim-lua/kickstart.nvim) ![](https://img.shields.io/github/commit-activity/y/nvim-lua/kickstart.nvim)

## Backwards Compatibility

- [weilbith/nvim-lsp-bacomp](https://github.com/weilbith/nvim-lsp-bacomp) ![](https://img.shields.io/github/stars/weilbith/nvim-lsp-bacomp) ![](https://img.shields.io/github/last-commit/weilbith/nvim-lsp-bacomp) ![](https://img.shields.io/github/commit-activity/y/weilbith/nvim-lsp-bacomp)
