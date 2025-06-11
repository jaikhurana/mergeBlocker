# mergeBlocker

if ! git config --global --get merge.fail.driver >/dev/null; then
  git config --global merge.fail.driver false
  echo "✅ Git merge driver 'fail' configured globally (driver = false)."
else
  echo "ℹ️ Git merge driver 'fail' is already set."
fi
