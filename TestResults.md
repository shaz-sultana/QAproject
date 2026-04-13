TC-API-001: GET /api/tasks
Expected: 200 OK with list of tasks
Actual: 200 OK — 3 tasks returned correctly
Pass/Fail: PASS ✓
TC-API-002: POST /api/tasks
Expected: 201 Created with new task
Actual: [what you see]
Pass/Fail: [PASS or FAIL]
TC-API-003: GET /api/tasks/1
Expected: 200 OK with task details
Actual: [what you saw]
Pass/Fail: [PASS or FAIL]
TC-API-004: GET /api/tasks/9999
Expected: 404 Not Found
Actual: [what you saw]
Pass/Fail: [PASS or FAIL]
TC-API-005: PUT /api/tasks/1
Expected: 200 OK with updated task
Actual: [what you saw]
Pass/Fail: [PASS or FAIL]
TC-API-006: DELETE /api/tasks/3
Expected: 204 No Content
Actual: [what you saw]
Pass/Fail: [PASS or FAIL]

## Summary

Total Tests: 6
Passed: 6
Failed: 0
Bugs Found: 0
