<script setup lang="ts">
import { Info } from 'lucide-vue-next'
import { useExportSupportDialog } from '@/features/editor/model'
import { Button } from '@/shared/ui/button'
import {
  Dialog,
  DialogContent,
  DialogDescription,
  DialogHeader,
  DialogTitle,
} from '@/shared/ui/dialog'

const { exportSupportDialogVisible, closeExportSupportDialog } = useExportSupportDialog()

function onOpenChange(open: boolean) {
  if (!open && exportSupportDialogVisible.value)
    closeExportSupportDialog()
}
</script>

<template>
  <Dialog
    :open="exportSupportDialogVisible"
    @update:open="onOpenChange"
  >
    <DialogContent class="sm:max-w-[460px]">
      <div
        class="mx-auto flex size-12 items-center justify-center rounded-full bg-primary/10 text-primary"
      >
        <Info class="size-6" />
      </div>

      <DialogHeader class="text-center sm:text-center">
        <DialogTitle>MobiWave Signature Card</DialogTitle>
        <DialogDescription class="leading-6">
          Create consistent, professional HTML email signatures for MobiWave Innovations Ltd.
          The tool is based on MySigMail Card, an open-source email signature editor.
        </DialogDescription>
      </DialogHeader>

      <div class="rounded-md border px-4 py-3 text-sm leading-6 text-muted-foreground">
        <strong class="text-foreground">MobiWave Innovations Ltd</strong><br>
        Kenya · Telecom + AI + Digital Infrastructure<br>
        Designed for MobiWave team signatures across email platforms and devices.
      </div>

      <Button
        variant="outline"
        @click="closeExportSupportDialog"
      >
        Continue
      </Button>
    </DialogContent>
  </Dialog>
</template>
