# Scala Best Practices

[![Join the chat at https://gitter.im/alexandru/scala-best-practices](https://badges.gitter.im/alexandru/scala-best-practices.svg)](https://gitter.im/alexandru/scala-best-practices?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

<img src="https://raw.githubusercontent.com/monifu/scala-best-practices/master/assets/scala-logo-256.png"  align="right" width="100" height="100" />

A collection of best practices, friendly to people that want to contribute. Forked from [alexandru/scala-best-practices](https://github.com/alexandru/scala-best-practices) and adapted to the typelevel stack.

- Version: `1.2`
- Updated at: `2016-06-08`

## Table of Contents

- [0. Preface](sections/0-preface.md)
  - [0.1 MUST NOT follow advice blindly](sections/0-preface.md#01-must-not-follow-advice-blindly)

- [1. Hygienic Rules](sections/1-hygienic-rules.md)
  - [1.1. SHOULD enforce a reasonable line length](sections/1-hygienic-rules.md#11-should-enforce-a-reasonable-line-length)
  - [1.2. MUST NOT rely on a SBT or IDE plugin to do the formatting for you](sections/1-hygienic-rules.md#12-must-not-rely-on-a-sbt-or-ide-plugin-to-do-the-formatting-for-you)
  - [1.3. SHOULD break long functions](sections/1-hygienic-rules.md#13-should-break-long-functions)
  - [1.4. MUST NOT introduce spelling errors in names and comments](sections/1-hygienic-rules.md#14-must-not-introduce-spelling-errors-in-names-and-comments)
  - [1.5. Names MUST be meaningful](sections/1-hygienic-rules.md#15-names-must-be-meaningful)

- [2. Language Rules](sections/2-language-rules.md)
  - [2.1. MUST NOT use "return"](sections/2-language-rules.md#21-must-not-use-return)
  - [2.2. SHOULD use immutable data structures](sections/2-language-rules.md#22-should-use-immutable-data-structures)
  - [2.3. SHOULD NOT update a "var" using loops or conditions](sections/2-language-rules.md#23-should-not-update-a-var-using-loops-or-conditions)
  - [2.4. SHOULD NOT define useless traits](sections/2-language-rules.md#24-should-not-define-useless-traits)
  - [2.5. MUST NOT use "var" inside a case class](sections/2-language-rules.md#25-must-not-use-var-inside-a-case-class)
  - [2.6. SHOULD NOT declare abstract "var" members](sections/2-language-rules.md#26-should-not-declare-abstract-var-members)
  - [2.7. MUST NOT throw exceptions for validations of user input or flow control](sections/2-language-rules.md#27-must-not-throw-exceptions-for-validations-of-user-input-or-flow-control)
  - [2.8. MUST NOT catch Throwable](sections/2-language-rules.md#28-must-not-catch-throwable-when-catching-exceptions)
  - [2.9. MUST NOT use "null"](sections/2-language-rules.md#29-must-not-use-null)
  - [2.10. MUST NOT use "Option.get"](sections/2-language-rules.md#210-must-not-use-optionget)
  - [2.11. MUST NOT use Java's Date or Calendar, instead use `java.time` (JSR-310)](sections/2-language-rules.md#211-must-not-use-javas-date-or-calendar-instead-use-javatime-jsr-310)
  - [2.12. SHOULD NOT use Any or AnyRef or isInstanceOf / asInstanceOf](sections/2-language-rules.md#212-should-not-use-any-or-anyref-or-isinstanceof--asinstanceof)
  - [2.13. MUST serialize dates as either Unix Timestamp or ISO 8601](sections/2-language-rules.md#213-must-serialize-dates-as-either-unix-timestamp-or-as-iso-8601)
  - [2.14. MUST NOT use magic values](sections/2-language-rules.md#214-must-not-use-magic-values)
  - [2.15. SHOULD NOT use "var" as shared state](sections/2-language-rules.md#215-should-not-use-var-as-shared-state)
  - [2.16. Public functions SHOULD have an explicit return type](sections/2-language-rules.md#216-public-functions-should-have-an-explicit-return-type)
  - [2.17. SHOULD NOT define case classes nested in other classes](sections/2-language-rules.md#217-should-not-define-case-classes-nested-in-other-classes)
  - [2.18. MUST NOT include classes, traits and objects inside package objects](sections/2-language-rules.md#218-must-not-include-classes-traits-and-objects-inside-package-objects)
  - [2.19. SHOULD use head/tail and init/last decomposition only if they can be done in constant time and memory](sections/2-language-rules.md#219-should-use-head-tail-and-init-last-decomposition-only-if-they-can-be-done-in-constant-time-and-memory)
  - [2.20. MUST NOT use `Seq.head`](sections/2-language-rules.md#210-must-not-use-seqhead)
  - [2.21. Case classes SHOULD be final](sections/2-language-rules.md#221-case-classes-should-be-final)
  - [2.22. SHOULD NOT use `scala.App`](sections/2-language-rules.md#222-should-not-use-scalaapp)


---

## Contribute

Open an issue to make suggestions, or create a pull request ;-)

---

Copyright &copy; 2015-2016, Some Rights Reserved.<br />
Licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
