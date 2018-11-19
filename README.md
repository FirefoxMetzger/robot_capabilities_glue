# Robot Capabilities Adapter

This small repo provides a website which changes the names of URL parameters to couple Amazon Mechanical Turk and the Unipark survey tool. 

The idea is that MTurk's external question provides 4 URL parameters when calling an external website: `assignmentId`, `hitId`, `turkSubmitTo`, `workerId`, but Unipark can only understand primitive alphabeticial variables: `a`, `b`, `c`, `d`. Hence, this page replaces MTurk names with single letters to be picked up by Unipark and then forwards to the newly created url.

You can configure Unipark to recognize URL parameters under `Survey options > User-defined variables` and then use them via `#p_0001`, `#p_0002`, ...
