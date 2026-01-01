# rust_training

Цель: подготовить рабочую среду для изучения Rust и предоставить простой пример проекта.

## Что сделано ✅
- Установлен `rustup` и стабильный toolchain Rust (включая `rustfmt` и `clippy`).
- Добавлены настройки для VS Code и рекомендации расширений (`rust-analyzer`, `crates`).
- Создан примерный проект `hello_rust` (lib) с тестами и успешно пройден `cargo test`.

---

## Быстрая инструкция по настройке (локально)
1. Установите rustup (если ещё не установлен):

   curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

   Затем выполните:

   source $HOME/.cargo/env

2. Установите дополнительные компоненты (опционально):

   rustup component add rustfmt clippy

3. Откройте репозиторий в VS Code и установите рекомендуемые расширения (справа внизу появится рекомендация) или вручную: `rust-lang.rust-analyzer`, `serayuzgur.crates`.

4. Создание и запуск примера:

   cd hello_rust
   cargo build
   cargo test

## Полезные команды
- Сборка: `cargo build`
- Запуск тестов: `cargo test`
- Форматирование: `cargo fmt`
- Проверки Clippy: `cargo clippy`

---

## Ресурсы
- Официальная документация Rust: https://doc.rust-lang.org/
- rust-analyzer: https://rust-analyzer.github.io/

Если хотите, могу добавить GitHub Action, который будет запускать `cargo test` на каждом push.
