# TIL
나의 첫번째 TIL 
CASE WHEN 문법을 ORDER BY 에서 사용이 가능 DECODE & CASE WHEN

STATUS = 1~3 의 값을 가지고 있을때
---------------------DECODE ----------------------------
DECODE (STATUS , NULL,'0', 1,2,3)
STATUS가 NULL 일경우 0번째 1일경우 2번째 둘다 아닐경우 3으로
---------------------CASE WHEN ----------------------------
CASE WHEN 문으로 작성할경우

ORDER BY CASE WHEN STATUS IS NULL THEN '0'
WHEN STATUS = '1' THEN 1,2
ELSE STATUS
END
