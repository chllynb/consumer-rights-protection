# Scenario: Hotel And OTA Booking Disputes

Use this file for hotel listings, room-type disputes, hidden occupancy limits, cancellation refusals, or booking-page descriptions that do not match the real stay conditions.

## Typical Fact Patterns

- The listing says "double room" or shows two beds, but the hotel refuses two guests.
- The page hides a material restriction such as occupancy, breakfast, window type, or check-in condition.
- The platform refuses refund solely based on a cancellation deadline even though the listing was misleading.
- The platform or hotel says "free cancellation before 18:00, non-refundable after 18:00" and refuses to review why the stay could not proceed.
- The room differs materially from the listing photos or promised amenities.

## Core Evidence

- Order page and order number
- Listing screenshots, especially room type and occupancy wording
- Photos or recordings at check-in
- Chat and call records with the hotel and platform
- Platform cancellation rules and timestamps
- Payment record showing the merchant or platform entity

If the dispute involves an 18:00 cutoff, also preserve:

- The exact cancellation-rule screenshot with timestamp
- The time when the user discovered the real issue
- The time when the user first contacted the hotel or platform
- Any proof that the hotel or platform caused or disclosed the problem too late

## Best Legal Framing

Usually combine:

- Misleading advertising or incomplete disclosure
- Unfair standard terms if the platform relies on rigid cancellation rules despite its own listing problem
- Failure to perform as agreed

Read:

- `references/legal-basis.md`
- `references/complaint-channels.md`

## Special Pattern: "Free cancellation before 18:00, non-refundable after 18:00"

This is a common hotel and OTA rule. Treat it as a standard term, not an automatic legal win for the merchant.

### When the merchant is in a stronger position

- The room information, occupancy, breakfast, and restrictions were clearly disclosed before payment
- The user simply changed plans for personal reasons after the cutoff
- The hotel remained able to perform exactly as advertised

In that case, a full refund argument is weaker, and the user may need to negotiate goodwill rather than insist on a guaranteed refund.

### When the consumer is in a stronger position

- The listing omitted or buried a material restriction
- The page gave a room impression that a normal consumer would reasonably misunderstand
- The hotel changed conditions after booking
- The user discovered the issue only because the merchant or platform disclosed it late
- The user never checked in and the stay failed due to inaccurate or incomplete listing information

In that case, argue that:

- The problem is not a simple late cancellation
- The booking purpose failed because of misleading or incomplete information
- The merchant or platform should not mechanically apply the 18:00 cutoff clause

### Fast Response Plan

1. Screenshot the cancellation rule, room page, and every material promise
2. Preserve the first message or call time when the issue was raised
3. Tell the platform the dispute is about listing accuracy or undisclosed restrictions, not a voluntary late cancellation
4. Ask the platform to escalate manual review instead of automatic rule enforcement
5. If refused, file 12315 using both "misleading information" and "unfair standard term" framing

## Merchant / Platform Message Template

```text
我于[日期]通过[平台]预订了[酒店名称][房型]，订单号[XXX]，支付[XXX]元。下单页面展示或足以使普通消费者理解为[宣传内容]，但实际情况为[实际情况]，与页面关键信息不符。

本次订单目的无法实现，原因在于页面信息存在误导、重大遗漏或重要限制未充分披露，并非我单方无故取消。请在24小时内提供处理方案，并按实际情况办理全额退款或合理补偿。
```

## Merchant / Platform Message Template For 18:00 Cutoff Cases

```text
我并非在明知房型信息准确、酒店可正常履约的情况下单纯超过18:00后反悔取消，而是因为下单页面对[房型/入住人数/限制条件/其他关键信息]展示不准确或披露不充分，导致我在[发现时间]才得知真实情况。

在贵方页面信息存在问题或重要信息披露不足的情况下，机械适用“18:00后不可退”规则并不合理。本人未实际入住，订单目的无法实现，请提交人工复核并办理退款。
```

## 12315 Complaint Template

```text
投诉人于[日期]通过[平台名称]预订[酒店名称][房型]，订单号[XXX]，支付金额[XXX]元。

问题在于：下单页面展示或足以使普通消费者理解为[宣传内容]，但实际到店后酒店或平台告知[实际情况]，导致订单目的无法实现。投诉人未实际消费入住，却被以“超过取消时限”等格式化规则拒绝退款。

投诉人认为，被投诉人存在页面信息不真实、不完整或引人误解的问题，并在自身存在过错的情况下援引不公平格式条款限制消费者退款权利。

诉求：
1. 退还订单费用[XXX]元；
2. 核查页面宣传及退款规则适用是否存在违法违规问题；
3. 督促被投诉人依法处理并反馈结果。

证据包括：订单截图、页面宣传截图、沟通记录、现场情况照片、录音等。
```

## 12315 Complaint Template For 18:00 Cutoff Cases

```text
投诉人于[日期]通过[平台名称]预订[酒店名称][房型]，订单号[XXX]，金额[XXX]元。平台页面展示或未充分提示的关键信息为[页面内容]，投诉人于[发现时间]得知实际情况为[实际情况]，导致订单目的无法实现。

投诉人未实际入住，并已于[时间]第一时间联系平台或酒店要求处理，但被机械适用“18:00前可退、18:00后不可退”等格式规则拒绝退款。

投诉人认为，本案核心争议并非单纯逾期取消，而是页面信息存在误导、重大遗漏或与实际履行条件不符。请求贵部门核查被投诉人的页面展示和退款规则适用是否合规，并督促退还订单费用[XXX]元。
```

## Practical Advice

- If the user never checked in, say that clearly.
- Focus on the mismatch between page information and actual conditions.
- Do not spend most of the complaint arguing "I changed my mind"; argue that the transaction failed because the listing was misleading or incomplete.
- In 18:00 cutoff cases, the key question is why the order failed, not only when the cancellation request was submitted.
