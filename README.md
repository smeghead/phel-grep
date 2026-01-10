# phel-grep

![Testing](https://github.com/smeghead/phel-grep/actions/workflows/ci.yml/badge.svg?event=push)

Programs that function as phel CLI commands execute as compiled PHP code at runtime, presenting unique challenges for handling command-line arguments.
Additionally, there are multiple ways to execute phel scripts (`phel run <scriptname>`, `phel run <namespace>`).

Therefore, simply using PHP's getopt does not work as expected in this context.

When creating CLI commands with phel, we developed a getopt library that provides natural command-line argument parsing.

