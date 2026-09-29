# tKAS, POCencept, and KUSDT

Three ways to pay on the [Kworld](https://sixpack.wtf/kworld.html) square. All three are Testnet-10 toys. None of them is a bank transfer, a dollar in a wallet, or Tether.

This note is why each rail exists, and how a shop spend moves. The square itself is described in [STP-KAS/kworld](https://github.com/STP-KAS/kworld).

## Why three

The point is the choice. Proof of work can carry a native coin, a proof-of-concept stable tag, and a tether-style tag that can be frozen. Putting them on one counter makes the difference visible. It does not make any of them a SEPA rail.

**tKAS** is the native Testnet-10 coin. It is the only one of the three that actually moves. A shop payment is a transaction to the village reserve. The miner fee is extra and is not part of the price.

**POCencept** is a proof-of-concept stable tag. The practice comes from Gramlane, Ishum, PegLab, and BitCoffee. This desk did not re-mint those assets. Grams are prepaid mass, not a dollar. PegLab is the classroom where a thin peg breaks. Ishum quotes a price and settles KAS. BitCoffee is a Testnet-10 covenant dollar that stays where it was written. POCencept is the tag on this square, quoted in toy cents, so a shop can be paid without moving tKAS.

**KUSDT** is a testnet tether-style tag in the same ledger. It exists so a freeze switch can be seen. Freeze blocks KUSDT only. POCencept and tKAS still pay. KUSDT is not Tether and it is not a claim on a dollar.

## How a price becomes a payment

Shops quote toy cents. Coffee is 250 cents. Supper is 1400. A lap of the square is 10000. The tag stays at those cents when the KAS price moves.

For tKAS, the till converts cents with the live KAS/USD quote from the public price feed. The page shows that quote. The transaction pays the reserve. A short payment is refused. The same transaction cannot mint the tag twice.

The bank locks tKAS into POCencept or KUSDT at that same quote. Redeem sends tKAS back only for the locked portion. The practice purse, which the bank can hand out, burns at the shop first and does not redeem. A failed redeem rolls the toy balance back, so a lock cannot be cashed twice.

Spending rules can refuse a shop, refuse a rail, cap the day, or ask for a second yes above a line. The second yes is checked before a test-tab key is allowed to sign.

## Where the ideas come from

- [gramlane](https://github.com/STP-KAS/gramlane)
- [gramlanepeglab](https://github.com/STP-KAS/gramlanepeglab)
- [peglab-stp](https://github.com/STP-KAS/peglab-stp)
- [peglab-poc](https://github.com/STP-KAS/peglab-poc)
- [ishum](https://github.com/STP-KAS/ishum)
- [kusdt-bitcoffee](https://github.com/STP-KAS/kusdt-bitcoffee)
- [poc-revisited](https://github.com/STP-KAS/poc-revisited)
- [kcc-importance](https://github.com/STP-KAS/kcc-importance)
- [kaspa-till](https://github.com/STP-KAS/kaspa-till)
- [Rails on sixpack.wtf](https://sixpack.wtf/rails.html)

KCC-20 is still Draft. Do not treat USDT or USDC as the unit or the fee of this square. There is no spendable layer-1 stable in this till.

## Covenants

BitCoffee's Testnet-10 dollar is a covenant. The network holds the rule. This square did not re-mint that coin.

POCencept and KUSDT here are rows in the village ledger. A freeze on KUSDT is a switch in that ledger. It is not a covenant script, and it does not freeze tKAS.

The confirm line is the stand-in for a covenant's second yes: over the line, the till waits. A SilverScript covenant would put that wait in the script that guards the coins, the way the Kaspero Labs freelancer sheet holds a payment until a milestone is notarized. The studio in that sheet does not hold the funds. Kworld's server does hold the toy ledger. That is the gap.

- [kaspanet/silverscript](https://github.com/kaspanet/silverscript)
- [Freelancer sheet](https://silverscriptstudio.com/freelancer.html)
- [Kaspero Labs](https://x.com/KasperoLabs/status/2104543100634886578)

## vProgs

A vProg guest, in the early prototype, applies one declared step and can be checked against that step. The tic-tac-toe guest does that for a ply. A shop spend could one day be the same kind of step: this address, this shop, this rail, this amount, accepted or refused.

Today the village ledger is a server. GitHub Pages cannot run it. The tic-tac-toe match does not settle coffee. Sequencing a till inside a guest is future work, not a claim this square makes.

- [biryukovmaxim/vprog-tictactoe](https://github.com/biryukovmaxim/vprog-tictactoe)
- [kaspanet/vprogs](https://github.com/kaspanet/vprogs)
- [STP-KAS/declared-ply](https://github.com/STP-KAS/declared-ply)
