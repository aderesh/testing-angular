This is a sample project of basic VS Code debugging configuration to debug Angular *.spec.ts files.

Reference: https://github.com/microsoft/vscode-recipes/tree/master/Angular-CLI

To debug unit tests (check `VSCodeAngularDebugging.gif`):
1. Run 'npm run test' in the terminal. Karma Chrome window should appear.
2. From the debug pane select `ng test`, press F5 or press the green button. New chrome window should appear.
3. Set a breakpoint in app.component.spec.ts.
4. Refresh the `http://localhost:9876/debug.html` Chrome window
5. The breakpoint should be hit.


There may be an issue with the breakpoint - it's not hit or it's marked as inactive. In this case:
1. Follow all the steps above
2. In the second chrome window open DevsToools
3. Open `Sources` tab
4. Open `top/localhost:9876/_karma_webpack_/src/app/app.component.spec.ts`
5. Put a breakpoint 
6. Refresh the `http://localhost:9876/debug.html` Chrome window

VS Code breakpoints should start working again.
