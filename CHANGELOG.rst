Development version
===================

 - add on_done keyword argument to specify a callback on all tasks
   (including the ThreadableTasks like fs operations).
 - sessionmanager.wait_for_tasks now wait for tasks that are started from
   other tasks callbacks from different sessions.

0.1.3 / 2015-06-16
==================

 - finished_callback, timeout_callback, stdout_callback and stderr_callback
   from command parameters are renamed to on_finished, on_timeout,
   on_stdout, on_stderr. Old names are still working for compatibility,
   they will be removed later - runtime warnings are issued for that.
 - session.wait_for_tasks now wait for tasks that are started from other
   tasks callbacks

0.1.2 / 2015-06-15
==================

 - keep silent errors around (errors that happened on tasks finished
   without explicit wait call)
 - add a copy_dir method on Session objects
 - add synchrone methods for copying files and directories
 - fix exception handling in ThreadableTask
 - add licence infornation (LGPL)
 - update documentation

0.1.1 / 2015-06-09
==================

 - fixed a bug with remote tasks (python typo)
 - remove task that timed out from the session tasks
 - update documentation

0.1.0 / 2015-06-08
==================

 - initial release
