const moment = require("moment-timezone");
const fs = require("fs");

moment.tz.setDefault("Asia/Jakarta").locale("id");

let dt = moment(Date.now()).tz('Asia/Jakarta').locale('id').format('a')
const ucapanWaktu = "Selamat "+dt.charAt(0).toUpperCase() + dt.slice(1)
let setting = JSON.parse(fs.readFileSync('./config.json'))
let hitbot = JSON.parse(fs.readFileSync('./database/dashboard/userhit.json'));
let pendaftar = JSON.parse(fs.readFileSync('./database/user.json'))

exports.menuall = (sender, prefix, pushname, ucapanWaktu, tanggal, jam, isOwner) => {
return `*OTHERS MENU*
 *≻* ${prefix}simi
 *≻* ${prefix}getpp
 *≻* ${prefix}listsewa
 *≻* ${prefix}cekprem
 *≻* ${prefix}listprem
 *≻* ${prefix}buyprem
 *≻* ${prefix}daftarprem
 
*MAIN MENU*
 *≻* ${prefix}id
 *≻* ${prefix}hit
 *≻* ${prefix}limit
 *≻* ${prefix}rules
 *≻* ${prefix}stats
 *≻* ${prefix}listgc
 *≻* ${prefix}listpc
 *≻* ${prefix}owner
 *≻* ${prefix}script
 *≻* ${prefix}server
 *≻* ${prefix}buylimit
 *≻* ${prefix}cekuser
 *≻* ${prefix}runtime
 *≻* ${prefix}dashboard

*PREMIUM MENU*
 *≻* ${prefix}rika
 *≻* ${prefix}bocil
 *≻* ${prefix}ghea
 *≻* ${prefix}hijab
 *≻* ${prefix}asupan
 *≻* ${prefix}santuy
 *≻* ${prefix}q
 *≻* ${prefix}join
 *≻* ${prefix}brainly
 *≻* ${prefix}quoted
 *≻* ${prefix}getquoted
 *≻* ${prefix}react
 *≻* ${prefix}towame
 *≻* ${prefix}menfes
 *≻* ${prefix}menfess

*STORE MENU*
 *≻* ${prefix}list
 *≻* ${prefix}addlist
 *≻* ${prefix}dellist
 *≻* ${prefix}update
 *≻* ${prefix}tambah
 *≻* ${prefix}kurang
 *≻* ${prefix}kali
 *≻* ${prefix}bagi

*TOPUP OTOMATIS*
 *≻* ${prefix}gopay
 *≻* ${prefix}topupff

*PROSES/DONE*
 *≻* proses < reply chat >
 *≻* done < reply chat >
 *≻* ${prefix}setproses
 *≻* ${prefix}changeproses
 *≻* ${prefix}delsetproses
 *≻* ${prefix}setdone
 *≻* ${prefix}changedone
 *≻* ${prefix}delsetdone

*RESPON/MESSAGE*
 *≻* ${prefix}delrespon
 *≻* ${prefix}addrespon
 *≻* ${prefix}setrespon
 *≻* ${prefix}listrespon

*SET WELCOME/LEFT*
 *≻* ${prefix}getleft
 *≻* ${prefix}setleft
 *≻* ${prefix}delleft
 *≻* ${prefix}changeleft
 *≻* ${prefix}setwelcome
 *≻* ${prefix}delwelcome
 *≻* ${prefix}getwelcome
 *≻* ${prefix}changewelcome

*CEK USERNAME*
 *≻* ${prefix}nickff
 *≻* ${prefix}nickml
 *≻* ${prefix}nicksupersus

*ANONYMOUS CHAT*
 *≻* ${prefix}start
 *≻* ${prefix}stop
 *≻* ${prefix}next
 *≻* ${prefix}sendprofil
 *≻* ${prefix}anonymous

*GROUP SETTING*
 *≻* ${prefix}left on
 *≻* ${prefix}left off
 *≻* ${prefix}antilink on
 *≻* ${prefix}antilink off
 *≻* ${prefix}antiwame on
 *≻* ${prefix}antiwame off
 *≻* ${prefix}welcome on
 *≻* ${prefix}welcome off

*GROUP MENU*
 *≻* ${prefix}add
 *≻* ${prefix}kick
 *≻* ${prefix}linkgc
 *≻* ${prefix}infogc
 *≻* ${prefix}infogrup
 *≻* ${prefix}promote
 *≻* ${prefix}demote
 *≻* ${prefix}hidetag
 *≻* ${prefix}tagall
 *≻* ${prefix}open
 *≻* ${prefix}close
 *≻* ${prefix}ceksewa
 *≻* ${prefix}setppgc
 *≻* ${prefix}setppgc 'panjang'
 *≻* ${prefix}setnamegc
 *≻* ${prefix}setdesc
 *≻* ${prefix}revoke
 *≻* ${prefix}setclose
 *≻* ${prefix}setopen
 *≻* ${prefix}delclose
 *≻* ${prefix}delopen
 *≻* ${prefix}getopen
 *≻* ${prefix}getclose

*OWNER MENU*
 > evalcode
 x evalcode-2
 $ executor
 *≻* ${prefix}bc
 *≻* ${prefix}join
 *≻* ${prefix}left
 *≻* ${prefix}self
 *≻* ${prefix}public
 *≻* ${prefix}sendsesi
 *≻* ${prefix}creategc
 *≻* ${prefix}setppbot
 *≻* ${prefix}setthumb
 *≻* ${prefix}broadcast
 *≻* ${prefix}listwaktu
 *≻* ${prefix}block 628xxx
 *≻* ${prefix}unblock 628xxx
 *≻* ${prefix}setppbot 'panjang'
 *≻* ${prefix}sewa del <waktu>
 *≻* ${prefix}sewa add <waktu>
 *≻* ${prefix}delprem @tag
 *≻* ${prefix}addprem @tag <waktu>

*RESTART DATABASE*
 *≻* ${prefix}resetlist
 *≻* ${prefix}resetall
 *≻* ${prefix}resethit
 *≻* ${prefix}resetkey
 *≻* ${prefix}resetuser
 *≻* ${prefix}resetbalance

*CONVERT/TOOLS*
 *≻* ${prefix}say
 *≻* ${prefix}tts
 *≻* ${prefix}ttp
 *≻* ${prefix}attp
 *≻* ${prefix}font
 *≻* ${prefix}font2
 *≻* ${prefix}isgd
 *≻* ${prefix}tourl
 *≻* ${prefix}cuttly
 *≻* ${prefix}tinyurl
 *≻* ${prefix}ssweb
 *≻* ${prefix}shorturl

*GENERATE TEXT*
 *≻* ${prefix}hilih
 *≻* ${prefix}halah
 *≻* ${prefix}huluh
 *≻* ${prefix}heleh
 *≻* ${prefix}holoh

*ENCODE/DECODE*
 *≻* ${prefix}base32
 *≻* ${prefix}base64
 *≻* ${prefix}debase32
 *≻* ${prefix}debase64

*PRIMBON MENU*
 *≻* ${prefix}artinama
 *≻* ${prefix}nomorhoki
 *≻* ${prefix}ramaljodoh
 *≻* ${prefix}suamiistri
 *≻* ${prefix}ramalcinta
 *≻* ${prefix}artimimpi
 *≻* ${prefix}sifatusaha
 *≻* ${prefix}cocoknama
 *≻* ${prefix}tafsirmimpi
 *≻* ${prefix}ramaljodohbali
 *≻* ${prefix}cocokpasangan

*RANDOM ANIME*
 *≻* ${prefix}ass
 *≻* ${prefix}ana
 *≻* ${prefix}akira
 *≻* ${prefix}asuna
 *≻* ${prefix}ahegao
 *≻* ${prefix}akiyama
 *≻* ${prefix}aesthetic
 *≻* ${prefix}deidara
 *≻* ${prefix}ayuzawa
 *≻* ${prefix}elaina
 *≻* ${prefix}emilia
 *≻* ${prefix}hinata
 *≻* ${prefix}isuzu

*RANDOM MENU*
 *≻* ${prefix}loli
 *≻* ${prefix}dare
 *≻* ${prefix}bucin
 *≻* ${prefix}truth
 *≻* ${prefix}meme
 *≻* ${prefix}couple
 *≻* ${prefix}jokes
 *≻* ${prefix}quotes
 *≻* ${prefix}cecan
 *≻* ${prefix}cogan
 *≻* ${prefix}anime

*COSPLAY RANDOM*
 *≻* ${prefix}cosplay
 *≻* ${prefix}cosplayloli
 *≻* ${prefix}cosplaysagiri

*DOWNLOAD MENU*
 *≻* ${prefix}play
 *≻* ${prefix}musik
 *≻* ${prefix}tiktok
 *≻* ${prefix}ytmp3
 *≻* ${prefix}ytmp4
 *≻* ${prefix}gitclone
 *≻* ${prefix}mediafire
 *≻* ${prefix}sosmed
 *≻* ${prefix}facebook
 *≻* ${prefix}soundcloud

*CONVERT STICKER*
 *≻* ${prefix}sticker <reply image>
 *≻* ${prefix}toimg <reply sticker>
 *≻* ${prefix}toimage <reply sticker>
 *≻* ${prefix}tovid <reply sticker gif>
 *≻* ${prefix}tovideo <reply sticker gif>
 
*ISLAMIC MENU*
 *≻* ${prefix}ayatkursi
 *≻* ${prefix}doaharian
 *≻* ${prefix}asmaulhusna
 *≻* ${prefix}bacaansholat

*GAMES MENU*
 *≻* ${prefix}tekateki
 *≻* ${prefix}tebaklirik
 *≻* ${prefix}tebakkata
 *≻* ${prefix}susunkata
 *≻* ${prefix}tebakgame
 *≻* ${prefix}caklontong
 *≻* ${prefix}siapakahaku
 *≻* ${prefix}tebakkalimat
 *≻* ${prefix}tebakgambar
 *≻* ${prefix}tebaktebakan

*MAKER MENU*
 *≻* ${prefix}nulis
 *≻* ${prefix}logo1
 *≻* ${prefix}logo2
 *≻* ${prefix}logo3
 *≻* ${prefix}emojimix
 *≻* ${prefix}emojimix2

*IMAGE EDITOR*
 *≻* ${prefix}hitler
 *≻* ${prefix}putin
 *≻* ${prefix}resize
 *≻* ${prefix}police
 *≻* ${prefix}petimati
 *≻* ${prefix}smeme
 *≻* ${prefix}discordblue
 *≻* ${prefix}discordblack

*SEARCHING MENU*
 *≻* ${prefix}lirik
 *≻* ${prefix}corona
 *≻* ${prefix}covid
 *≻* ${prefix}cerpen
 *≻* ${prefix}jadwaltv
 *≻* ${prefix}salurantv
 *≻* ${prefix}stalkgithub
 *≻* ${prefix}pinterest
 *≻* ${prefix}styletext
 *≻* ${prefix}infogempa
 *≻* ${prefix}wikimedia
 *≻* ${prefix}gimage
 *≻* ${prefix}google
 *≻* ${prefix}ringtone
 *≻* ${prefix}gsmarena
 *≻* ${prefix}quotesanime`
}

exports.textprem  = (sender, prefix) => {
return `Jika kamu ingin menjadi Member Premium, kamu cukup membayar 
Rp5.000 untuk 1 Minggu
Rp20.000 untuk 1 Bulan 
dan jika ingin menjadi Member Premium Permanen kamu hanya membayar Rp50.000. Jika berminat silahkan chat Owner Bot, ketik ${prefix}owner

*Payment :* 
Dana/Qris/Ovo`
}

exports.textdonasi = (sender, prefix) => {
return `*DONASI BOT*

*E-walet Monay :*
➭ Dana : 0857-2749-2435
➭ Ovo : 0857-2749-2435
➭ Gopay : 08xxxxxxxxx
➭ Bca : 3570844228
    
*Qris All Payment :*
https://telegra.ph/qrallpayment-08-30-2`
}