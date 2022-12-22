# pharmacokinetics
## Background
本計算器用來評估

現行皮質素(cortisol)的檢驗多為免疫分析法。
在服用外源性類固醇的情況下，可能因為交叉反應導致 cortisol 的結果假性偏高。
以現行檢驗技術而言，檢驗誤差一般而言不至於影響醫療絕測。
然而，針對本計算器用來粗估使用口服皮質醇，對於血液 cortisol 的干擾程度。

本計算器使用藥物動力學模型預估類固醇藥物之血中濃度，

口服藥物使用one compartment model, first order kinetic作為預測模型。

## Limitation
正確地理解檢驗方法有助於正確的臨床解讀。

 1. 預測濃度不宜當作真值
    - 檢驗的交叉反應是由血液中藥物濃度得出。
    - 本計算器預估之交叉反應**不宜**用來推測真實的藥物與皮質素濃度。正確的理解方式，是**此濃度預估了檢驗項目的干擾程度**。使用者應綜合皮質素結果與臨床情境，決定該次檢驗之可信度。
    - 真正的血中藥物濃度仍應由直接檢驗測得，請用真正的直接測量
 2. 交叉反應參數隨試驗廠牌有所差異
    - 不同廠牌試劑因為設計之抗體不同，對於各物質有不同交叉反應。
    - 本計算器預估之交叉反應(現今林口長庚紀念醫院採用廠牌)，**對於他牌皮質素檢驗僅能作為參考**。
 3. 類固醇藥物動力學可能隨濃度有差異
    - 本計算機中 prednisolone, metylprednisolone 之藥物動力學參數隨著濃度不同有所差異。

同一個檢驗項目的交叉反應會隨試劑廠牌有所差異，
檢驗方法
plasma cortisol 的檢驗使用 The Elecsys Cortisol II assay 作為參考。
在此試劑中，交叉反應較明顯的藥物為 prednisolone 和 methylpredisolone。
注意到交叉反應的程度因為試劑不同，不得直接轉換。

本計算器得出數值對於

## Reference
 1. Czock, D et al, (2005). Pharmacokinetics and pharmacodynamics of systemically administered glucocorticoids. Clinical pharmacokinetics, 44(1), 61-98.
 2. Roche Diagnostics. Cortisol: Method Sheet. (https://pim-eservices.roche.com)
