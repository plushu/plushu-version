#!/usr/bin/env bash
set -eo pipefail; [[ -n "$PLUSHU_TRACE" ]] && set -x

case "$1" in
  --version)
    if [[ -d "$PLUSHU_ROOT/.git" ]]; then
      GIT_DIR="$PLUSHU_ROOT/.git" git describe
      exit 0
    else
      echo "No .git directory in $PLUSHU_ROOT, version unknown" >&2
      exit 1
    fi
    ;;
esac
