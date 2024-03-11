class Node:
    def init(self, nama_menu, harga):
        self.nama_menu = nama_menu
        self.harga = harga
        self.next = None

class LinkedList:
    def init(self):
        self.head = None

    def menambahkan_pesanan(self, nama_menu, harga):
        new_node = Node(nama_menu, harga)
        if not self.head:
            self.head = new_node
        else:
            current = self.head
            while current.next:
                current = current.next
            current.next = new_node

 def menampilkan_pesanan(self):
        current = self.head
        if not current:
            print("Keranjang kosong")
        else:
            print("Pesanan:")
            while current:
                print(f"{current.nama_menu}: Rp{current.harga}")
                current = current.next

    def menghitung_total(self):
        harga_total = 0
