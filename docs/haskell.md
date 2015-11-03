# Haskell

函数式编程

---

## 安装（Arch Linux）

```bash
sudo pacman -Syu # 更新系统
sudo pacman -S ghc # 编译器
sudo pacman -S cabal-install # 包管理
sudo pacman -S haddock # 文档生成
sudo pacman -S happy # Parser generator
sudo pacman -S alex # Lexical analyzer generator
```

## 配置

### spacemacs

```sh
cabal install hlint # consume a lot of resources
cabal install stylish-haskell
cabal install hasktags
cabal install ghc-mod
cabal install structured-haskell-mode
cabal install hindent
```

### Vim

```text
Plugin 'lukerandall/haskellmode-vim'
```

## 读书笔记

### Learn You a Haskell for Great Good!

### Real World Haskell

### Yesod Web Framework Book
