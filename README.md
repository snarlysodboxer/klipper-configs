# Klipper on Smoothieboard on Azteeg X5 GT

This is for my Pulse XE from Matterhackers

## Status
Still a work in progress
Can now home all axes

Motors were getting way too hot, I finally made this change to the klipper code as a test, and it fixed it
```python
--- a/klippy/extras/tmc2660.py
+++ b/klippy/extras/tmc2660.py
@@ -155,7 +155,8 @@ class TMC2660CurrentHelper:
                 if abs(run_current - cur2) < abs(run_current - cur):
                     vsense = False
                     irun = irun2
-        return vsense, irun
+        #  return vsense, irun
+        return True, 14
```
