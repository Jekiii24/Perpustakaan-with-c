# Perpustakaan-with-c


#include <stdio.h>
#include <string.h>

int main()
{
    int harga_buku_novel, pil_buku, kode_buku_novel, kode_buku_cerpen, Kode_buku_pel, kode_buku_ins, i = 1;
    int total_pembelian = 0, total_bayar, bayar, kembalian;
    char kar_novel = 'y', kar_cerpen = 'y', kar_jenis_buku = 'y', kar_buku_pel = 'y', kar_buku_ins = 'y';
    char nama[20];

    printf("\t\t====================================================================\n");
    printf("\t\t\t||    SELAMAT DATANG DI PERPUSTAKAAN JAYA MAKMUR    ||\n");
    printf("\t\t\t||                 BUDAYAKAN MEMBACA                ||\n");
    printf("\t\t\t||             ENJOY AND HAPPY READING!!            ||\n");
    printf("\t\t====================================================================\n");

    printf("\t~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n");

    printf("Siapa nih nama kakak, boleh dong kenalan dulu :D\n\n");
    printf("Masukan nama anda : ");
    scanf("%s", &nama);

    printf("Halo kak %s, Mau pesen buku apa ? \n\n", nama);

    while (kar_jenis_buku == 'y')
    {
        printf("\t\t||        -- Jenis Buku --       ||\n\n");
        printf("\tSilahkan Pilih jenis buku yang ingin anda pesan\n");
        printf("\t1.Novel\n");
        printf("\t2.Cerpen\n");
        printf("\t3.Buku pelajaran\n");
        printf("\t4.Buku inspiratif\n");
        printf("\tMasukan pilihan anda(1-4) : ");
        scanf("%d", &pil_buku);
        printf("\n");
        getchar();

        if (pil_buku == 1)
        {
            printf("\t--Ini dia daftar buku novel--\n");
            printf("\t1.Home sweet loan - Almira bastari\n");
            printf("\t2.Laut bercerita - Leila S. Chudori\n");
            printf("\t3.Sagaras - Tere Liye\n");
            printf("\t4.Layangan putus - MOMMY ASF\n");
            printf("\t5.Different - Kadek Pingetania\n");
            printf("\t6.Janji - Tere Liye\n");
            printf("\t7.Ancika - Pidi Baiq\n");
            printf("\t8.Septihan - Poppi Pertiwi\n");
            printf("\t9.Senja dan pagi - Allfy Rev\n");
            printf("\t10.Jingga dan Senja - Esti Kinasih\n\n");

            printf("Masukan nomor barang yang ingin anda beli\n");

            while (kar_novel == 'y')
            {
                printf("\tBarang ke - %d : ", i);
                scanf("%d", &kode_buku_novel);
                getchar();

                if (kode_buku_novel == 1)
                {
                    harga_buku_novel = 80000;
                    printf("\tHome sweet loan - Almira bastari\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_novel == 2)
                {
                    harga_buku_novel = 135000;
                    printf("\tLaut bercerita - Leila S. Chudori\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_novel == 3)
                {
                    harga_buku_novel = 100000;
                    printf("\tSagaras - Tere Liye\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_novel == 4)
                {
                    harga_buku_novel = 75000;
                    printf("\tLayangan putus - MOMMY ASF\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_novel == 5)
                {
                    harga_buku_novel = 50000;
                    printf("\tDifferent - Kadek Pingetania\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_novel == 6)
                {
                    harga_buku_novel = 105000;
                    printf("\tJanji - Tere Liye\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_novel == 7)
                {
                    harga_buku_novel = 80000;
                    printf("\tAncika - Pidi Baiq\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_novel == 8)
                {
                    harga_buku_novel = 100000;
                    printf("\tSeptihan - Poppi Pertiwi\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_novel == 9)
                {
                    harga_buku_novel = 95000;
                    printf("\tSenja dan pagi - Allfy Rev\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_novel == 10)
                {
                    harga_buku_novel = 70000;
                    printf("\tJingga dan Senja - Esti Kinasih\n\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else
                {
                    printf("\tKode barang salah!\n");
                    continue;
                }

                total_pembelian = total_pembelian + harga_buku_novel;
                printf("\t           ---Reminder---          \n");
                printf("\tJika anda keluar dari laman ini, anda tidak bisa memesan buku yang ada di laman ini lagi\n\n");
                printf("\tIngin memesan buku novel lainnya? [y/t] = ");
                scanf(" %c", &kar_novel);
                getchar();
                printf("\n");
                i++;
            }
        }
        else if (pil_buku == 2)
        {
            printf("\t--Ini dia daftar buku cerpen--\n");
            printf("\t1.Sepotong Senja untuk Pacarku - Seno Gumira Ajidarma\n");
            printf("\t2.Seribu Kunang-kunang di manhattan - Umar Kayam\n");
            printf("\t3.Robohnya Surau kami - A. A. Navis\n");
            printf("\t4.Maukah Kau Menghapus Bekas Bibirnya di Bibirku dengan Bibirmu? - Hamsad Rangkuti\n");
            printf("\t5.Dilarang Mencintai Bunga-Bunga - Kuntowijoyo\n");
            printf("\t6.Anjing-Anjing Menyerbu Kuburan - Kuntowijoyo\n");
            printf("\t7.Lukisan Kaligrafi - A. Mustofa Bisri\n");
            printf("\t8.Senyum Karyamin - Ahmad Tohari\n");
            printf("\t9.Godlob - Danarto\n");
            printf("\t10.Tegak Lurus dengan Langit - Iwan Simatupang\n\n");

            printf("Masukan nomor barang yang ingin anda beli\n");

            while (kar_cerpen == 'y')
            {
                printf("\tBarang ke - %d : ", i);
                scanf("%d", &kode_buku_cerpen);
                getchar();

                if (kode_buku_cerpen == 1)
                {
                    harga_buku_novel = 70000;
                    printf("\tSepotong Senja untuk Pacarku - Seno Gumira Ajidarma\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_cerpen == 2)
                {
                    harga_buku_novel = 135000;
                    printf("\tSeribu Kunang-kunang di manhattan - Umar Kayam\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_cerpen == 3)
                {
                    harga_buku_novel = 100000;
                    printf("\tRobohnya Surau kami - A. A. Navis\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_cerpen == 4)
                {
                    harga_buku_novel = 75000;
                    printf("\tMaukah Kau Menghapus Bekas Bibirnya di Bibirku dengan Bibirmu? - Hamsad Rangkuti\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_cerpen == 5)
                {
                    harga_buku_novel = 50000;
                    printf("\tDilarang Mencintai Bunga-Bunga - Kuntowijoyo\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_cerpen == 6)
                {
                    harga_buku_novel = 105000;
                    printf("\tAnjing-Anjing Menyerbu Kuburan - Kuntowijoyo\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_cerpen == 7)
                {
                    harga_buku_novel = 80000;
                    printf("\tLukisan Kaligrafi - A. Mustofa Bisri\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_cerpen == 8)
                {
                    harga_buku_novel = 100000;
                    printf("\tSenyum Karyamin - Ahmad Tohari\n");

                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_cerpen == 9)
                {
                    harga_buku_novel = 95000;
                    printf("\tGodlob - Danarto\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_cerpen == 10)
                {
                    harga_buku_novel = 70000;
                    printf("\tTegak Lurus dengan Langit - Iwan Simatupang\n\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else
                {
                    printf("\tKode barang salah!\n");
                    continue;
                }
                total_pembelian = total_pembelian + harga_buku_novel;
                printf("\t           ---Reminder---          \n");
                printf("\tJika anda keluar dari laman ini, anda tidak bisa memesan buku yang ada di laman ini lagi\n\n");
                printf("\tIngin memesan buku cerpen lainnya? [y/t] = ");
                scanf(" %c", &kar_cerpen);
                getchar();
                printf("\n");
                i++;
            }
        }
        else if (pil_buku == 3)
        {
            printf("\t--Ini dia daftar buku pelajaran--\n");
            printf("\t1.Ipa (Kimia) - kurikulum merdeka\n");
            printf("\t2.Fisika\n");
            printf("\t3.Biologi\n");
            printf("\t4.Matematika (Peminatan)\n");
            printf("\t5.Matematika (Wajib)\n");
            printf("\t6.Bahasa Indonesia\n");
            printf("\t7.Bahasa Inggris\n");
            printf("\t8.Ekonomi\n");
            printf("\t9.Geografi\n");
            printf("\t10.Sosiologi\n\n");

            printf("Masukan nomor barang yang ingin anda beli\n");

            while (kar_buku_pel == 'y')
            {
                printf("\tBarang ke - %d : ", i);
                scanf("%d", &Kode_buku_pel);
                getchar();

                if (Kode_buku_pel == 1)
                {
                    harga_buku_novel = 150000;
                    printf("\tIpa (Kimia) - kurikulum merdeka\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (Kode_buku_pel == 2)
                {
                    harga_buku_novel = 75000;
                    printf("\tFisika\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (Kode_buku_pel == 3)
                {
                    harga_buku_novel = 60000;
                    printf("\tBiologi\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (Kode_buku_pel == 4)
                {
                    harga_buku_novel = 90000;
                    printf("\tMatematika (Peminatan)\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (Kode_buku_pel == 5)
                {
                    harga_buku_novel = 170000;
                    printf("\tMatematika (Wajib)\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (Kode_buku_pel == 6)
                {
                    harga_buku_novel = 100000;
                    printf("\tBahasa Indonesia\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (Kode_buku_pel == 7)
                {
                    harga_buku_novel = 115000;
                    printf("\tBahasa Inggris\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (Kode_buku_pel == 8)
                {
                    harga_buku_novel = 70000;
                    printf("\tEkonomi\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (Kode_buku_pel == 9)
                {
                    harga_buku_novel = 50000;
                    printf("\tGeografi\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (Kode_buku_pel == 10)
                {
                    harga_buku_novel = 85000;
                    printf("\tSosiologi\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else
                {
                    printf("\tKode barang salah!\n");
                    continue;
                }
                total_pembelian = total_pembelian + harga_buku_novel;
                printf("\t           ---Reminder---          \n");
                printf("\tJika anda keluar dari laman ini, anda tidak bisa memesan buku yang ada di laman ini lagi\n\n");
                printf("\tIngin memesan buku cerpen lainnya? [y/t] = ");
                scanf(" %c", &kar_buku_pel);
                getchar();
                printf("\n");
                i++;
            }
        }
        else if (pil_buku == 4)
        {
            printf("\t--Ini dia daftar buku inspiratif--\n");
            printf("\t1.Almost Adulting: Self-Help Approach to Deal With Quarter-Life Crisis - NADHIRA AFIFA\n");
            printf("\t2.Overheard Jakarta - OVERHEARDJKT\n");
            printf("\t3.Pijar Psikologi Yang Belum Usai: Kenapa Manusia Punya Luka Batin - Pijar Psikologi\n");
            printf("\t4.Buku Stop Overthinking: Lebih Happy Jalani Hidup dengan Tidak Berpikir Berlebih - Nick Trenton\n");
            printf("\t5.The Art Of Thinking Clearly - Rolf Dobelli\n");
            printf("\t6.Generation Gap(less): Seni Menjalin Relasi Antargenerasi - Erwin Parengkuan & Becky Tumewu\n");
            printf("\t7.Nanti Juga Sembuh Sendiri - Helo Bagas\n");
            printf("\t8.Merawat Luka Batin - Dr Jiemi Ardian\n");
            printf("\t9.Ego Is The Enemy - Ryan Holiday\n");
            printf("\t10.Berani Tidak Disukai - Ichiro Kishimi Dan Fumitake Koga\n\n");

            printf("Masukan nomor barang yang ingin anda beli\n");

            while (kar_buku_ins == 'y')
            {
                printf("\tBarang ke - %d : ", i);
                scanf("%d", &kode_buku_ins);
                getchar();

                if (kode_buku_ins == 1)
                {
                    harga_buku_novel = 90000;
                    printf("\tAlmost Adulting: Self-Help Approach to Deal With Quarter-Life Crisis - NADHIRA AFIFA\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_ins == 2)
                {
                    harga_buku_novel = 90000;
                    printf("\tOverheard Jakarta - OVERHEARDJKT\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_ins == 3)
                {
                    harga_buku_novel = 55000;
                    printf("\tPijar Psikologi Yang Belum Usai: Kenapa Manusia Punya Luka Batin - Pijar Psikologi\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_ins == 4)
                {
                    harga_buku_novel = 55000;
                    printf("\tBuku Stop Overthinking: Lebih Happy Jalani Hidup dengan Tidak Berpikir Berlebih - Nick Trenton\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_ins == 5)
                {
                    harga_buku_novel = 140000;
                    printf("\tThe Art Of Thinking Clearly - Rolf Dobelli\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_ins == 6)
                {
                    harga_buku_novel = 75000;
                    printf("\tGeneration Gap(less): Seni Menjalin Relasi Antargenerasi - Erwin Parengkuan & Becky Tumewu\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_ins == 7)
                {
                    harga_buku_novel = 67000;
                    printf("\tNanti Juga Sembuh Sendiri - Helo Bagas\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_ins == 8)
                {
                    harga_buku_novel = 78000;
                    printf("\tMerawat Luka Batin - Dr Jiemi Ardian\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_ins == 9)
                {
                    harga_buku_novel = 95000;
                    printf("\tEgo Is The Enemy - Ryan Holiday\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else if (kode_buku_ins == 10)
                {
                    harga_buku_novel = 78000;
                    printf("\tBerani Tidak Disukai - Ichiro Kishimi Dan Fumitake Koga\n");
                    printf("\tHarga buku : %d\n\n", harga_buku_novel);
                }
                else
                {
                    printf("\tKode barang salah!\n");
                    continue;
                }
                total_pembelian = total_pembelian + harga_buku_novel;
                printf("\t           ---Reminder---          \n");
                printf("\tJika anda keluar dari laman ini, anda tidak bisa memesan buku yang ada di laman ini lagi\n\n");
                printf("\tIngin memesan buku inspirasi lainnya? [y/t] = ");
                scanf(" %c", &kar_buku_ins);
                getchar();
                printf("\n");
                i++;
            }
        }
        printf("Ingin memesan jenis buku lainnya? [y/t] = ");
        scanf(" %c", &kar_jenis_buku);
        getchar();
        printf("\n");
    }

    printf("\t==============================================================================================\n");
    printf("\t\t\t\t\t\tSTRUK PEMBAYARAN\n");
    printf("\t==============================================================================================\n");
    printf("\tNama Anda                                                 : %s\n", nama);
    printf("\tTotal Pembayaran anda                                     : Rp.%d\n", total_pembelian);
    printf("\tSilahkan masukan uang anda                                : Rp.");
    scanf("%d", &bayar);
    kembalian = bayar - total_pembelian;
    printf("\tKembalian anda sebesar                                    : Rp.%d\n\n", kembalian);

    printf("Terimakasih sudah mampir ke perpustakaan jaya makmur :D\n");
    printf("Jangan lupa tetap membaca buku dari perpustakaan kami ya\n");
    printf("HAPPY READING!!!!!\n");

    return 0;
}
