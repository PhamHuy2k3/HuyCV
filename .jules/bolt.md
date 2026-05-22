## 2024-05-22 - Optimizing React List Keys
**Learning:** While using unique identifiers instead of array indices for React `key` props is a standard best practice to optimize DOM reconciliation, it yields zero measurable performance benefit for statically defined lists that never change at runtime.
**Action:** When evaluating React component performance, distinguish between static and dynamic lists before applying reconciliation micro-optimizations, as static lists are already handled efficiently by index keys.
